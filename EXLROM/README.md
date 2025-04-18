# EXLROM Multi-ROM Cartridge
## Summary
The Exelvision EXL100 (and Exeltel) cartridge port pinout is below - the B-side face up and A-side face down when the cartridge is inserted.<br>
The pinout was determined from the 32KByte Tennis cartridge.  The A1 pin was not connected in this cartridge but is connected to pin 40 of the TAL004 gate array ... perhaps a 2nd ROM select line?<br>
```
A1 = ROMCS2(?)  B1 = ROMCS1
A2 = A13        B2 = A14
A3 = A11        B3 = A12
A4 = A9         B4 = A10
A5 = A7         B5 = A8
A6 = A5         B6 = A6
A7 = GND        B7 = A4
A8 = N/C        B8 = +5V
A9 = A3         B9 = A2
A10 = A1        B10 = A0
A11 = D7        B11 = D6
A12 = D5        B12 = D4
A13 = D3        B13 = D2
A14 = D1        B14 = D0
```
## [Simple Single ROM Version](/EXLROM/EXLROM_256Kbit/)
This version takes a 32KByte 27C256 EPROM that will fit a single 32KByte ROM.  The smaller 8KByte and 16KByte ROMs will just have empty space.<br>

## [Multi-ROM](/EXLROM/EXLROM_4Mbit/)
This version should fit all known Exelvision ROMs.<br>

## Bank Selection
Using a 4MBit EPROM allows us to fit 16 32KByte ROMs selectable via four dip switches that determine the value of the A15 to A18 address lines.  A single ROM can be created by concatenating 32KByte ROMs into one file - very simply done in Linux or Windows via command line.  Smaller ROMs (8KByte and 16KByte) can be duplcated (i.e. four concatenated copies of the 8KByte ROM) to bring their size up to 32KBytes.
```
AAAA 
1111
8765 Bank  ROM Address Range
---- ----  -----------------
0000    0  0x00000-0x07FFF
0001    1  0x08000-0x0FFFF
0010    2  0x10000-0x17FFF
0011    3  0x18000-0x1FFFF
0100    4  0x20000-0x27FFF
0101    5  0x28000-0x2FFFF
0110    6  0x30000-0x37FFF
0111    7  0x38000-0x3FFFF
1000    8  0x40000-0x47FFF
1001    9  0x48000-0x4FFFF
1010   10  0x50000-0x57FFF
1011   11  0x58000-0x5FFFF
1100   12  0x60000-0x67FFF
1101   13  0x68000-0x6FFFF
1110   14  0x70000-0x77FFF
1111   15  0x78000-0x7FFFF
```
## Cartridge Pinout
The B-side that faces up when inserted.  Pins are numbered B1 on the right to B14 on left.<br>
![Cartridge B-side](/Images/EXL100_Cartridge_B.jpg)
The A-side that faces down when inserted.  Pins are numbered A1 on the right and A14 on the left.<br>
![Cartridge A-side](/Images/EXL100_Cartridge_A.jpg)
