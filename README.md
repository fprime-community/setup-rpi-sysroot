# setup-rpi-sysroot: setup RPI builds with optional SYSROOT

This will download and install the given toolchain archive to the directory specified in RPI_TOOLCHAIN_DIR. It will
optionally loopback the supplied sysroot image such that it may be used.

## Inputs

| input            | default                                          | description                |
|------------------|--------------------------------------------------|----------------------------|
| toolchain        | Linaro GCC for ARM GNU/Linux 32bin w/ Hard Float | Toolchain To Download      |
| sysroot-image    | **unused**                                       | SYSROOT Image to download  |
| sysroot-location | `/tmp/rpi-sysroot`                               | Directory to place sysroot |

## Linaro Toolchain

The default toolchain is the Linaro 7.5 toolchain.  This is because this toolchain is known to work with Raspberry PI Os
images as of the late 2022 Debian 11 based releases.  The toolchain is available at:
[Linaro 7 Latest](https://releases.linaro.org/components/toolchain/binaries/latest-7/arm-linux-gnueabihf/)