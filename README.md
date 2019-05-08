# melonDS

DS emulator, sorta
Okay, i just want to improve and practice my C and HW theory skills.
All thanks to Rinnegatamante, hardest things is primary things.

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

 * use CodeBlocks
 * or receive golden cookies if you get Cmake to work (i don`t get this shit)

## TODO LIST (MY OWN)

 * improve  UI, more config things.
 * Перевести на православный Russian и, возможно, не менее крутющий German.На второй язык - наверное.
 * More like DraStic all things.
 * HWA

 
## Credits
 * Rinnegatamante for platform to make things (and others)
