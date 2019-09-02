# melonDS

DS emulator, sorta
Okay, i just want to improve and practice my C and HW theory skills.
All thanks to Rinnegatamante, hardest things is primary things.
For now im currently ran out of memory of my vita (32 gb microSD + vita sd card 16 gb).
Sorry for that, but im unable to test it for a while.
UPD: Got 64 Gb microSD and now im in!

The goal is to do things right and fast, akin to blargSNES (but hopefully better). But also to, you know, have a fun challenge :)

The source code is provided under the GPLv3 license.

## How to use

melonDS requires BIOS/firmware copies from a DS. Files required:
 * bios7.bin, 16KB: ARM7 BIOS
 * bios9.bin, 4KB: ARM9 BIOS
 * firmware.bin, 128/256/512KB: firmware
 
Firmware boot requires a firmware dump from an original DS or DS Lite.
DS firmwares dumped from a DSi or 3DS aren't bootable and only contain configuration data, thus they are only suitable when booting games directly.

### Possible firmware sizes

 * 128KB: DSi/3DS DS-mode firmware (reduced size due to lacking bootcode)
 * 256KB: regular DS firmware
 * 512KB: iQue DS firmware

DS BIOS dumps from a DSi or 3DS can be used with no compatibility issues. DSi BIOS dumps (in DSi mode) are not compatible. Or maybe they are. I don't know.

As for the rest, the interface should be pretty straightforward. If you have a question, don't hesitate to ask, though!

## How to build

### Linux:

```sh
mkdir -p build
cd build
cmake ..
make
```

### Windows:
YEEEEEE I tried and now i can compile this homebrew from windows.
Here is the guide:
- Windows 10 required
- Install linux (google it)
- Run bash (cmd -> bash command)
- Install vitaSDK with linux way.
set vitaSDK to path:
export VITASDK=/usr/local/vitasdk
export PATH=$VITASDK/bin:$PATH
(i dont know why but i have to do path exports every time i run bash)
- now if vitaSDK properly installed, run 
echo $VITASDK
and if you correct, it must type path to vitasdk folder.
- Now compile:
cd to_where_you_want_your_project
- Run git clone https://github.com/mrdivdiz/melonDS-Vita-div.git
- Install 7zip ("sudo apt-get install p7zip-full")
- Run mkdir -p build (make "build" dir)
- Run make
if there is param.sfo error, just put param.sfo to /build and run make again
- VPK ready, just install it
(If that compile way is strange, thats okay, im a newbie)

Rinnegatamante windows (any version) ways:
 * use CodeBlocks
 * or receive golden cookies if you get Cmake to work (i don`t get this shit)

## TODO LIST (MY OWN)

 * improve  UI, more config things.
 * Перевести на православный Russian и, возможно, не менее крутющий German.На второй язык - наверное.
 * More like DraStic all things.
 * HWA
 * Make Time Hollow and CoD Black Ops work perfectly (maybe)

 
## Credits
 * Rinnegatamante for platform to make things (and others)
