# Fractal Design Hackintosh

## Software

- **macOS High Sierra 10.13.3**
- Clover Clover v2.4k r4920
- Clover Global Configurator 5.4.3.1

## Hardware
* **Case:** Fractal Design R5
* **CPU:** Intel Core i7-4790K
* **Motherboard:** Gigabyte z97x-ud5h
    F8 BIOS
    ALC1150 Audio
	Qualcomm Atheros Killer E2201 LAN
	Intel i217V LAN
* **WiFi:** TP-LINK Archer T8E AC1750
* **Storage:** Samsung 840 PRO SSD
* **Graphics:** EVGA GTX 1060 6GB

## What Works
* Sleep, shutdown, and restarting works
* Have not tested USB3 yet and am using USB2 for sound
* Full graphics acceleration with the NVidia Web Drivers / Cuda Drivers
* "About this Mac" correctly reports memory and graphics.

This system is running stable for the most part. Since I had TONS of issues getting this running on Sierra, I thought I'd put this up here to help other people out. If anyone sees any room for improvement, let me know. I'm still in the process of tweaking this install.

## Issues
Please check the Github issue tracker for an up-to-date list of issues.

## Setup
1. Use TonyMac's guide to create a bootable USB: https://www.tonymacx86.com/threads/unibeast-install-macos-sierra-on-any-supported-intel-based-pc.200564/
2. Replace the Clover EFI folder with this one. Please back up Clover's default clover.plist, just in case
3. You may need to add `nv_disable=1` to my config.plist, since web drivers will not be installed at first
4. Install macOS Sierra (using TonyMac's guide)

## Mojave Upgrade?
* https://www.insanelymac.com/forum/topic/334334-wipsuccess-z97x-ud5h-i7-4770k-running-mojave-beta-1/
* https://www.tonymacx86.com/threads/readme-common-problems-and-workarounds-on-10-14-mojave.255823/
* Seems like WhateverGreen is starting to become the standard for Graphics Fixes.

## Similar Builds
* https://github.com/AlJohri/hackintosh/tree/master/atul
* https://www.tonymacx86.com/threads/success-build-macos-sierra-on-gigabyte-z97x-ud5h-i7-4770k-16gb-ram-gtx-760.215548/

## Useful Tools
* TonyMac DSDT Library and Forums
* Unibeast: create USB Installer
* Clover: awesome bootloader. Patches / adds stuff on the fly.
* Clover Configurator: easiest way to mount EFI partitions and edit config.plist.
* Nvidia Web Drivers
* https://github.com/Benjamin-Dobell/nvidia-update
* CUDA Drivers
* https://github.com/walkman2021/PC-DSDT-Patches/blob/master/Gigabyte/Z97X_UD5H.txt
