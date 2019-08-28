# libfixmath

The start of a libfixmath Particle library

Ported from: https://github.com/PetteriAimonen/libfixmath

## Unit testing

See src/demo.cpp for the unit tests.

## Known Errors

I am currently getting the following liker errors when attempting to build this project for the Photon:

```
/home/nrobinson/.po-util/bin/gcc-arm-embedded/gcc-arm-none-eabi-5_3-2016q1/bin/../lib/gcc/arm-none-eabi/5.3.1/../../../../arm-none-eabi/lib/armv7-m/libg_nano.a(lib_a-writer.o): In function `_write_r':
writer.c:(.text._write_r+0x10): undefined reference to `_write'
/home/nrobinson/.po-util/bin/gcc-arm-embedded/gcc-arm-none-eabi-5_3-2016q1/bin/../lib/gcc/arm-none-eabi/5.3.1/../../../../arm-none-eabi/lib/armv7-m/libg_nano.a(lib_a-closer.o): In function `_close_r':
closer.c:(.text._close_r+0xc): undefined reference to `_close'
/home/nrobinson/.po-util/bin/gcc-arm-embedded/gcc-arm-none-eabi-5_3-2016q1/bin/../lib/gcc/arm-none-eabi/5.3.1/../../../../arm-none-eabi/lib/armv7-m/libg_nano.a(lib_a-fstatr.o): In function `_fstat_r':
fstatr.c:(.text._fstat_r+0xe): undefined reference to `_fstat'
/home/nrobinson/.po-util/bin/gcc-arm-embedded/gcc-arm-none-eabi-5_3-2016q1/bin/../lib/gcc/arm-none-eabi/5.3.1/../../../../arm-none-eabi/lib/armv7-m/libg_nano.a(lib_a-isattyr.o): In function `_isatty_r':
isattyr.c:(.text._isatty_r+0xc): undefined reference to `_isatty'
/home/nrobinson/.po-util/bin/gcc-arm-embedded/gcc-arm-none-eabi-5_3-2016q1/bin/../lib/gcc/arm-none-eabi/5.3.1/../../../../arm-none-eabi/lib/armv7-m/libg_nano.a(lib_a-lseekr.o): In function `_lseek_r':
lseekr.c:(.text._lseek_r+0x10): undefined reference to `_lseek'
/home/nrobinson/.po-util/bin/gcc-arm-embedded/gcc-arm-none-eabi-5_3-2016q1/bin/../lib/gcc/arm-none-eabi/5.3.1/../../../../arm-none-eabi/lib/armv7-m/libg_nano.a(lib_a-readr.o): In function `_read_r':
readr.c:(.text._read_r+0x10): undefined reference to `_read'
collect2: error: ld returned 1 exit status
../../../build/module.mk:232: recipe for target '/home/nrobinson/projects/libfixmath/target/libfixmath.elf' failed
make[2]: *** [/home/nrobinson/projects/libfixmath/target/libfixmath.elf] Error 1
../build/recurse.mk:11: recipe for target 'modules/photon/user-part' failed
make[1]: *** [modules/photon/user-part] Error 2
/home/nrobinson/.po-util/src/particle.mk:34: recipe for target 'compile-user' failed
make: *** [compile-user] Error 2
```