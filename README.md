# ZXCU
A menu guided setup utility for ZX-Uno and settings set configurator. Allows to change several settings in the ZX-Uno on the fly, without reseting, and allows saving different profiles to restore them later.

## Build instructions
* Compile the BAS file with [ZX-Basic](http://www.boriel.com/wiki/en/index.php/ZXBasic) (requires Python to run):

  `python zxbc.py ZXUC.BAS -O9 -S 45000`

* Compile the ASM files with [Pasmo](http://pasmo.speccy.org/):

  `pasmo zxuc.asm ZXUC`
  `pasmo zxucsave.asm ZXUCSAVE`

* Copy the `ZXUC`, `ZXUCSAVE` and `ZXUC.BIN` files in the `/BIN` folder of your SD card. 

## Usage

ESXDOS: Put ZXUC, ZXUCSAVE and ZXUC.BIN files at you SD card /BIN folder 
UnoDOS: Put ZXUC, ZXUCSAVE and ZXUC.BIN files at you SD card /CMD folder 

* Open the GUI:

.zxuc

* Save the current settings to the named file (normal filename restrictions apply):

.zxucsave filename

* Restore previously saved settings:

 You can restore  previously saved profile typing:

.zxuc xxxxxxxx

Profile files are stored at /SYS/CONFIG/ZXUCCFG folder.



