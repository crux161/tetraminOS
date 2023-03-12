# TetraminOS: An operating system, but is mostly a space to play with tetraminos... Mostly...

![screenshot](images/0.png)

#### Features:
- It's basically a tetris clone... 
- 32-bit (x86) (working on that...)
- Fully custom bootloader
- ~~Soundblaster 16 driver~~ NO AUDIO (currently anyways...)
- ~~Custom music track runner~~ AGAIN.. ((SMH)) NO AUDIO!!!
- Fully hardcoded tetris theme (whatever TF that means...)
- Double-buffered 60 FPS graphics at 320x200 pixels with custom 8-bit RGB palette

#### Running
**NOTE**: This has *only* been tested in an emulator. Real hardware might not like it.

##### Mac OS
```
$ make iso
$ qemu-system-i386 -drive format=raw,file=boot.iso -d cpu_reset -monitor stdio 
```

##### LINUX (&WSL) / UNIX / ??? MinGW ??? 
```
$ make iso 
$ qemu-system-i386 -drive format=raw,file=boot.iso -d cpu_reset -monitor stdio
```
##### Windows
Working on this one, but as of right now -- there is no build system that wouldn't require the use of something like MinGW

##### Real hardware
Chances are writing this to a usb drive will cause it to boot, but all of that is just theory and has not been tested... YET.
