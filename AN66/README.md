# Building SF2000 1.6 Multicore on AN66
The bisrv in this folder is stock sf2000 1.6 with patched the buttons and screen. The buttons are the same as DY19 and the screen is the same as GB300.  
Methodology to make this bisrv:  
- Start with SF2000 1.6 firmware with GB300 screen swap
- Get the binary diffrence between SF2000 1.6 firmware on DY19 and the [SF2000 1.6 original firmware](https://github.com/Dteyn/Datafrog_SF2000_Vanilla/releases/tag/v1.6) to get the button patch
- Use the diff above to patch the SF2000 1.6 firmware with GB300 screen swap
- As always [patch crc](https://vonmillhausen.github.io/sf2000/tools/biosCRC32Patcher.htm)  

This uses the same screen as the gb300 so you must apply [this patch](https://github.com/tzubertowski/gb300_multicore/commit/0d8b553) when building multicore and all cores must be rebuilt.  
