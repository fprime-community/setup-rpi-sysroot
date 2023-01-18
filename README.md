# setup-rpi-sysroot: download and mount the RPI base (headless) image as a sysroot

This action uses `losetup` and `mount` to download the RPI base image, and mount it as a loopback device. 

## Inputs

Required where no default available.

| input    | default                                                                                                                                                 | description                |
|----------|---------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------|
| location | `$GITHUB_WORKSPACE/rpi-sysroot`                                                                                                                         | Directory to place sysroot |
| image    | [this image]("https://downloads.raspberrypi.org/raspios_lite_armhf/images/raspios_lite_armhf-2022-09-26/2022-09-22-raspios-bullseye-armhf-lite.img.xz") | RaspberryPI OS             |

