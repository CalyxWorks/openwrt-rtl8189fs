# OpenWrt RTL8189FS Driver

An out-of-tree Linux kernel driver project for Realtek RTL8189FS SDIO Wi-Fi adapters on OpenWrt.

## Project status

This project is in early development. The initial target is an Amlogic S905X P212 board running OpenWrt with the `6.18.56-ophub` kernel.

### Verified so far

- SDIO device ID: `024C:F179`
- Kernel module: `8189fs.ko`
- Wi-Fi scanning: successfully tested with the current development build
- IPS configuration: built with `RTW_IPS_MODE=0`

Scanning has been verified, but long-term connection stability, reconnection behavior, and automated builds remain to be tested.

## Compatibility

Compatibility is documented for specific combinations of hardware, OpenWrt build, kernel version, and driver configuration. Support for other devices and kernels is not implied.

## Build and distribution

The goal is to provide reproducible driver builds and clearly identify each build's target kernel and configuration. Prebuilt modules must only be used with compatible kernels.

## Licensing and acknowledgements

The driver is derived from existing Realtek RTL8189FS driver source. Original copyright notices and applicable license terms must be preserved. Licensing details will be documented after the source and license files have been verified.

## Disclaimer

This project is provided for testing and development. Wi-Fi functionality and stability may vary with hardware, firmware, kernel configuration, and access point. Back up your system before installing or replacing kernel modules.
