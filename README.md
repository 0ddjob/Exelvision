# Exelvision EXL100
Hardware projects and other info for the French Exelvision EXL100 computer.<br>
It has the following main ICs:
- Texas Instruments TMS4408 ... 8k x 4bit giving 32KBytes of shared VRAM
- NEC D4016 ... 2KByte SRAM for CPU RAM
- Texas Instruments TAL004 ... Gate Array
- Texas Instruments L30002N ... TMS 7220 CPU
- Texas Instruments C34802N ... TMS 7041 peripheral co-processor
- Texas Instruments TMP5220CNL ... TMS 5220 speech synthesiser
- Texas Instruments TMX3556NS ... TMS 3556 video display processor (VDP)

The ROM cartridge connector is a BURNDY PWBH14DER1A-1 which I can't find any info on - it's a 2x14 design.<br>

## YouTube Videos
- [Exelvision EXL100: Part 1 (First Look)](https://youtu.be/5-ew3FQ9LnI)
- [Exelvision EXL100: Part 2 (Cartridge Pinout)](https://youtu.be/ktFMq2L3tBw)
- [Simple Kicad For Simple Vintage Computer Hobbyists: Part 4 (ROM Cartridge Design)](https://youtu.be/U81MPNWrCRY)

## [EXLROM - Multi-ROM cartridge](/EXLROM/)
The EXL100 could accept ROM cartridges from 8KByte to 32KByte in size, including BASIC.  By using a 4Mbit ROM (27C040) we can fit all known ROMs onto one cartridge.  How exciting.<br>
I've designed two versions: a simple 256kbit version that will hold a single 32KByte ROM (like the olden days) and the 4Mbit version that will hold up to 16 32KByte ROMs.<br>
### Status
- 1-Apr-2025: Pending test fabrication 

![3D image of EXLROM 4MBit cartridge](/Images/EXLROM_4Mbit_3D.png)

## Partial TAL004 Gate Array Pinout
From cartridge pinout investigation ... <br>
![TAL004 partial pinout](/Images/EXL100_TAL004_partial_pintout.jpg)
