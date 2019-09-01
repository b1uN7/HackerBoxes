# HackerBoxes
Code for different H@ck3Rb0x3$
# B0X oo46 _Persistance_
[GxEPD_Example.ino](https://github.com/b1uN7/HackerBoxes/blob/master/GxEPD_Example.ino)

[IMG_0001.h](https://github.com/b1uN7/HackerBoxes/blob/master/IMG_0001.h)

## EPD MH-ET LIVE Resources:

Reading/How-To/Video:

[https://www.waveshare.com/wiki/1.54inch_e-Paper_Module#Demo_video](https://www.waveshare.com/wiki/1.54inch_e-Paper_Module#Demo_video)

Code that worked:

- First import library (with Library Manager in Arduino): GxEPD (NOT GxEPD2)

- Code:

By xxlucas42:

[https://gist.githubusercontent.com/xxlukas42/](https://gist.githubusercontent.com/xxlukas42/)

Example File:

[https://gist.github.com/xxlukas42/dab2cbd1202ce75b5d421490910e8639/raw/de44f61d8304a51dcae0667c227f05cf6a12bb6b/eink_demo.ino](https://gist.github.com/xxlukas42/dab2cbd1202ce75b5d421490910e8639/raw/de44f61d8304a51dcae0667c227f05cf6a12bb6b/eink_demo.ino)

EDITS to example .ino file:

- UNcomment line:

#include <GxGDEW0154Z04/GxGDEW0154Z04.h> // 1.54" b/w/r 200x200

- Confirm proper pinning on lines just above SETUP Function:

GxIO_Class io(SPI, /*CS=*/ SS, /*DC=*/ 8, /*RST=*/ 9);

GxEPD_Class display(io, /*RST=*/ 9, /*BUSY=*/ 7);

### NOTE: PINS 8 AND 9 ARE REVERSED IN DIFFERENT CODE!!  ENSURE YOU PINOUT CORRECTLY PER YOUR CODE!!!


