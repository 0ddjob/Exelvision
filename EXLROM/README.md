# EXLROM Multi-ROM Cartridge
## Summary
The Exelvision EXL100 (and Exeltel) cartridge port pinout is below - the B-side face up and A-side face down when the cartridge is inserted.<br>
The pinout was determined from the 32KByte Tennis cartridge.  The A1 pin was not connected in this cartridge but is connected to pin 40 of the TAL004 gate array ... perhaps a 2nd ROM select line?
```
A1 = N/C    B1 = ROM select
A2 = A13    B2 = A14
A3 = A11    B3 = A12
A4 = A9     B4 = A10
A5 = A7     B5 = A8
A6 = A5     B6 = A6
A7 = GND    B7 = A4
A8 = N/C    B8 = +5V
A9 = A3     B9 = A2
A10 = A1    B10 = A0
A11 = D7    B11 = D6
A12 = D5    B12 = D4
A13 = D3    B13 = D2
A14 = D1    B14 = D0
```
## Cartridge Pinout
The B-side that faces up when inserted.  Pins are numbered B1 on the right to B14 on left.<br>
![Cartridge B-side](/Images/EXL100_Cartridge_B.jpg)
The A-side that faces down when inserted.  Pins are numbered A1 on the right and A14 on the left.<br>
![Cartridge A-side](/Images/EXL100_Cartridge_A.jpg)
