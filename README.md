# Fractal Design Hackintosh

## Software

- **macOS High Sierra 10.13.3**
- Clover Clover v2.4k r4411
- Clover Configurator 4.60.2.0

## Hardware
* **Case:** Fractal Design R5
* **Motherboard:** Gigabyte z97x-ud5h (F8 BIOS)
* **CPU:** Intel Core i7-4790K
* **WiFi:** TP-LINK Archer T8E AC1750 (not using LAN)
* **Storage:** Samsung SSD 840 PRO SSD
* **Graphics:** EVGA GTX 1060 6GB

## What's Working
* Sleep, shutdown, and restarting works
* Have not tested USB3 yet and am using USB2 for sound
* Full graphics acceleration with the NVidia Web Drivers / Cuda Drivers
* "About this Mac" correctly reports memory and graphics.

This system is running stable for the most part. Since, I had TONS of issues getting this running on Sierra, I thought I'd put this up here to help other people out. If anyone sees any room for improvement, let me know. I'm still in the process of tweaking this install.

## What's Not Working
Please check the Github issue tracker for an up-to-date list of issues.

## Brief Instructions (not finished)
1. Use TonyMac's guide to create a bootable USB: https://www.tonymacx86.com/threads/unibeast-install-macos-sierra-on-any-supported-intel-based-pc.200564/
2. Replace the Clover EFI folder with this one. Please back up Clover's default clover.plist, just in case
3. You may need to add `nv_disable=1` to my config.plist, since web drivers will not be installed at first
4. Install macOS Sierra (using TonyMac's guide)

## Useful Tools
* TonyMac DSDT Library and Forums
* Unibeast: create USB Installer
* Clover: awesome bootloader. Patches / adds stuff on the fly.
* Clover Configurator: easiest way to mount EFI partitions and edit config.plist.
* Nvidia Web Drivers
* CUDA Drivers
