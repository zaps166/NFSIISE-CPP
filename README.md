NFSIISE-CPP
===========

This repository is a ASM->CPP translation of [NFSIISE](https://github.com/zaps166/NFSIISE).

This game can run on ARM devices, but it still uses Desktop OpenGL 1.x.
Currently it can run on Raspberry Pi 3 with open source VC4 graphics drivers.

The performance is about 2x - 2.5x lower than assembly code.
Also it can be less stable than assembly code due to possible translation bugs.
You can edit `~/.nfs2se/nfs2se.conf` and set `UseOnlyOneCPU` to `1`. This can improve the performance, but sometimes it can cause deadlocks.

###Requirements:
* SDL2 (32-bit) and Desktop OpenGL (32-bit),
* target must be 32-bit little-endian,
* GCC 4.9 or higher (not Clang).

###Cloning and compilation:
```
git clone https://github.com/zaps166/NFSIISE-CPP
cd NFSIISE-CPP
git submodule init
git submodule update
./compile_nfs
```

###Bug reporting:
Please report only translation bugs here.
If the same bug happens in assembly code, please report it into [main repository](https://github.com/zaps166/NFSIISE/issues/).

Please don't open PR's here, because the CPP file is auto-generated.
Open an issue instead and describe the problem :)
