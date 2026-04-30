# Versions

| MCU          | version          | Status               | Changes                               | Known issues                        |
| ------------ | ------------ | ------------------------ | ------------------------------------- | ------------------------------------- |
| ProMicro | 2025-10-08   | ✅Tested - Working 👍   |  First version  |   🤔NOT CRITICAL🤔<br><br>- Voltage divider labels are wrong, they are swapped. (B+ is B- and vice versa) <br><br> - Missing copper area on one side.       |                                       |
| ProMicro | 2025-11-04   | ✅Tested - Working 👍   |   - Voltage divider labels were fixed. <br><br> - Missing copper area was added. <br><br> - Added TLV840 voltage supervisor. <br><br>  - Added SI2312 mosfet for GPS.        |  - Negative boost pad misplaced.<br><br>  |
| S3 | 2025-11-21   | ✅Tested - Working ⁉️   |   - First version for ESP32 S3 SuperMini<br><br>- Should be compatible with C3 SuperMini too, but you'll loose controlling gps mosfet and battery sensing.)        |                                        |
| ProMicro | 2026-02-17   | ⁉️Tested - Working ⁉️   |   - Fix boost input pins<br><br> - Added caps <br><br> - Removed e80<br><br> - NEW Compact radio selector         |                                       |
| S3 | 2026-04-13   | ⁉️Tested - Working ⁉️   |   - Fix boost input pins<br><br> - Added caps<br><br> - NEW Compact radio selector        |                                        |
| ProMicro e80 | 2026-04-12   | ⁉️Tested - Working ⁉️   |   - First version       |                                       |
