# xiaoWa_pcb - 小瓦
A small watt pcb design compatible with [Meshtastic](https://meshtastic.org/)®.

# Pictures
<details><summary>Click to open</summary>

| Front | Back |
| :------------ | :---------------------------- |
|![image](https://github.com/gargomoma/xiaoWa_pcb/blob/main/pics/PCB_XiaoWa_2025-11-04_top.png) | ![image](https://github.com/gargomoma/xiaoWa_pcb/blob/main/pics/PCB_XiaoWa_2025-11-04_bottom.png) |

</details>

## Features
- Small size: 60 x 25 mm
- Compatible with Ebyte's E22; E22P and E80 radios.
- You can select between E22 or E22P with a solder bridge.
- 2mm mounting holes.
- Firmware is ProMicro DIY (same as FakeTec) 

## PCB Versions
- 2025-10-08 -> ✅Tested - Working 👍
- 2025-11-04 -> ⁉️Tested - Working ⁉️

Check [here](https://github.com/gargomoma/xiaoWa_pcb/tree/main/gerbers) for further info.

# Bill of materials
- WIP

# Notes

### Bootloader
>Check if the bootloader version is >0.8, update if needed from [here](https://github.com/adafruit/Adafruit_nRF52_Bootloader/releases)
>
>Look for: "update-nice_nano_bootloader-X.X.X_nosd" where X.X.X is the version.
>
>Latest version is: [update-nice_nano_bootloader-0.9.2_nosd.uf2](https://github.com/adafruit/Adafruit_nRF52_Bootloader/releases/download/0.9.2/update-nice_nano_bootloader-0.9.2_nosd.uf2)
>
>To flash all you need to do is to connect the device via USB and double tap RST and GND pins with tweezers. After doing so you should see in your OS a USB storage device named "NICENANO". Copy/move the .uf2 file into the storage device and wait for the reboot.
>
>If you cannot do this, consider the board came without bootloader, keep reading to know how to flash it.

### Charging current
>If you plan to charge the batteries, remember you can increase the charging current by bridging the _boost_ pads at the bottom of the proMicro board.
>You'll find more info on AliExpress listing, and also <a href="https://github.com/joric/nrfmicro/wiki/Alternatives#supermini-nrf52840l" target="_blank">here</a>.
>

### My ProMicro is dead. What can i do?
##### ⚠️ALWAYS TEST THE ProMicros BEFORE SOLDERING!⚠️
>Some sellers sell the ProMicros for very very cheap, but they don't provide bootloader (so you basically got a very smol brick), no problem.

Download the .hex bootloader from [here](https://github.com/adafruit/Adafruit_nRF52_Bootloader/releases) and prepare an ESP32 with the instructions provided [here](https://github.com/atc1441/ESP32_nRF52_SWD).

Latest .hex bootloader is [nice_nano_bootloader-0.9.2_s140_6.1.1.hex](https://github.com/adafruit/Adafruit_nRF52_Bootloader/releases/download/0.9.2/nice_nano_bootloader-0.9.2_s140_6.1.1.hex).

Once you got the ESP32 board ready, solder `CLK`,`DIO`,`GND`,`VDD` (or the `3v`) to the corresponding pins on the ESP32. (The ProMicro pins are on the back of the board.)

Then:
 1. Power the ESP32 on, on your browser open swd.local (or the IP assigned)
 2. Click Init SWD (if the "Status" shows not okay, check the wiring)
 3. Erase nRF -> Ok: Everything erased (if nRF info mentions locked, erase & reset)
 4. Flash Uploaded File -> Select file (the .hex bootloader), offset = 0
 5. Flash uploaded File; Wait for the upload to complete.
 6. 🧟‍♀️IT'S ALIVEEEE🧟‍♀️

# ♥Thanks♥
Thanks to all the folks using the fakeTec ♥ and specially to those who contributed to improve it. (Special shout out to lupusworax & ShimonHoranek )
Also thanks to Karman on the testing and improvement of the design.

# About Meshtastic
[Meshtastic](https://meshtastic.org/)® is a registered trademark of Meshtastic LLC. Meshtastic software components are released under various licenses, see github for details.

# Disclaimer
No warranty is provided.
You use it at your own risk and take the responsibility upon yourself.