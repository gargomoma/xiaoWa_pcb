# xiaoWa_pcb - 小瓦
A small watt node pcb design compatible with [Meshtastic](https://meshtastic.org/)®.

The pcb is designed to take as little space as possible, ideal for portable and hidden nodes. (You can fit it inside 32mm PVC pipes.)

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
- Recover from brownouts (TLV840)
- Mosfet to control external hardware (GPS)

## PCB Versions
- 2025-10-08 -> ✅Tested - Working 👍
- 2025-11-04 -> ⁉️Tested - Working ⁉️

Check [here](https://github.com/gargomoma/xiaoWa_pcb/tree/main/gerbers) for further info.

# Bill of materials

    You'll notice two links, both lead to the same product page.
    To support me, please use the 🤝 (referral links).

| Part | <div style="width:100px">Source</div>| Cost&nbsp;(€) | Note |
| :------------ | :------------------------------- | :-----------------| :-----------------|
| ProMicro (aka NiceNano) | <a href="https://www.aliexpress.com/item/1005006446457448.html" target="_blank">AliExpress</a><br /> <a href="https://www.aliexpress.com/item/1005007738886550.html" target="_blank">AliExpress</a> | 5€ <br /> 2x for 5€ | ⚠️[Review this before buying red ProMicros.](https://github.com/gargomoma/fakeTec_pcb/issues/30)<br> <a href="https://github.com/joric/nrfmicro/wiki/Alternatives#supermini-nrf52840l" target="_blank">⚠️ and also this.</a> |
| Ebyte E22P | <a href="https://es.aliexpress.com/item/1005009793885799.html" target="_blank">AliExpress</a> <br><a href="https://s.click.aliexpress.com/e/_ExCMka8" target="_blank">🤝AliExpress</a> | 10€ |  |
| Ebyte E22-XXXM30s | <a href="https://es.aliexpress.com/item/1005009741346732.html" target="_blank">AliExpress</a> <br><a href="https://s.click.aliexpress.com/e/_Ex353NQ" target="_blank">🤝AliExpress</a> | 10€ | M33S might work 🤔 |
| Ebyte E80 | <a href="https://es.aliexpress.com/item/1005007765300020.html" target="_blank">AliExpress</a> <br><a href="https://s.click.aliexpress.com/e/_EInpttQ" target="_blank">🤝AliExpress</a> | 7€ |  |
| 1206 SMD Resistor | <a href="https://www.aliexpress.com/item/1005006044241818.html" target="_blank">1- AliExpress</a><br><a href="https://s.click.aliexpress.com/e/_EG3dx2u" target="_blank">1- 🤝AliExpress</a> <br><br> <a href="https://www.aliexpress.com/item/1005002991902748.html" target="_blank">2- AliExpress</a><br><a href="https://s.click.aliexpress.com/e/_Ewlio7Q" target="_blank">2- 🤝AliExpress</a> | 3€ pack<br /> 0.1€/resistor | I'm using 2x 1M ohms.<br>Option 1: multiple values.<br>Option 2: choose your value. |
| Boost HW-085 | <a href="https://es.aliexpress.com/item/1005007592845254.html" target="_blank">AliExpress</a><br><a href="https://s.click.aliexpress.com/e/_ExA0hQo" target="_blank">🤝AliExpress</a> | 1.73€<br> pack of 5 | I'm using 2x 1M ohms |
| OLED SSD1306 i2c (optional) | <a href="https://es.aliexpress.com/item/1005007387721823.html" target="_blank">AliExpress</a><br><a href="https://s.click.aliexpress.com/e/_EGD8jBw" target="_blank">🤝AliExpress</a> | 1.5€ | No need to solder, just be careful and add some tape in between the boards to avoid a short. |
| SD05CRMA  (optional) | <a href="https://es.aliexpress.com/item/1005008971674620.html" target="_blank">AliExpress</a><br><a href="https://s.click.aliexpress.com/e/_EIGHi40" target="_blank">🤝AliExpress</a> | 2.5€<br> pack of 5 | Ideal if you'll insert it into a tube.<br>There's also a LifePo4 version. |
| TLV840  (optional) | <a href="https://es.aliexpress.com/item/1005009355692739.html" target="_blank">AliExpress</a> | 5€<br> pack of 10 | Ideal if you'll insert it into a tube.<br>There's also a LifePo4 version. |
| JST PH2.0 Battery connection (optional) | <a href="https://www.aliexpress.com/item/1005002564191148.html" target="_blank">AliExpress</a><br><a href="https://s.click.aliexpress.com/e/_EHICMko" target="_blank">🤝AliExpress</a> | 2€ pack<br /> 0.4€/unit | This is an example. |
| RG178 Antenna pigtail (recommended) | <a href="https://www.aliexpress.com/item/4001287491018.html" target="_blank">AliExpress</a><br><a href="https://s.click.aliexpress.com/e/_EzabLhq" target="_blank">🤝AliExpress</a> | 2€ | I saw that it underperformed with a cheap black pigtail, after using one of these, it worked fine. |
| PCB |  | 2€ pack of 5<br /> 0.4€/unit | Use your favourite company to get the PCB. |
| 2x Buttons | <a href="https://es.aliexpress.com/item/1005004380696913.html" target="_blank">AliExpress</a><br><a href="https://s.click.aliexpress.com/e/_EGIGFYM" target="_blank">🤝AliExpress</a> | 2.7€<br> pack of 50 | I couldn't find a part code, search for "3\*4\*2 2 Pin Button" |
| Mosfets SI2312 | <a href="https://www.aliexpress.com/item/1005004676217612.html" target="_blank">AliExpress</a><br><a href="https://s.click.aliexpress.com/e/_EGgKMLO" target="_blank">🤝AliExpress</a> | 9€ pack of 200<br /> | --- |
| &nbsp;&nbsp; | &nbsp;&nbsp; | &nbsp;&nbsp; | &nbsp;&nbsp; |
| <strong>Total</strong> |&nbsp;&nbsp; | 20€ | &nbsp;&nbsp; |

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
Thanks to all the folks using the fakeTec ♥ and specially to those who contributed to improve it.

(Special shout out to lupusworax & ShimonHoranek )

Also thanks to Karman on the testing and improvement of this design.

# About Meshtastic
[Meshtastic](https://meshtastic.org/)® is a registered trademark of Meshtastic LLC. Meshtastic software components are released under various licenses, see github for details.

# Disclaimer
No warranty is provided.
You use it at your own risk and take the responsibility upon yourself.