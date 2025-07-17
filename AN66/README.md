# SF2000 1.6 on AN66
[bisrv_SF2000_1.6_to_AN66.asd](https://github.com/Trademarked69/Frankenstein-Froggy-Firmware/blob/main/AN66/bisrv_SF2000_1.6_to_AN66.asd) is stock sf2000 1.6 with patched buttons and screen for AN66. The buttons are the same as DY19 and the screen is the same as GB300.  
Methodology to make this bisrv:  
- Start with [SF2000 1.6 firmware with GB300 screen swap](https://github.com/Trademarked69/Frankenstein-Froggy-Firmware/blob/main/SF2000/bisrv_GB300_screen_in_SF2000.asd)
- Get the binary diffrence between [SF2000 1.6 firmware on DY19](https://github.com/Trademarked69/Frankenstein-Froggy-Firmware/blob/main/DY19/bisrv_SF2000_1.6_to_DY19.asd) and the [SF2000 1.6 original firmware](https://github.com/Dteyn/Datafrog_SF2000_Vanilla/releases/tag/v1.6) to get the button patch
- Use the diff above to patch the SF2000 1.6 firmware with GB300 screen swap
- As always [patch crc](https://vonmillhausen.github.io/sf2000/tools/biosCRC32Patcher.htm)  

This uses the same screen as the GB300 so you must apply [this patch](https://github.com/tzubertowski/gb300_multicore/commit/0d8b553) when building SF2000 multicore and all cores must be rebuilt.  
