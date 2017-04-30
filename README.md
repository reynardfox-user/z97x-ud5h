# Fractal Design Hackintosh
Working Clover configuration for z97x-ud5h, i7-4790K, GTX 760

## System Specs
* Case: Fractal Design R5
* Motherboard: Gigabyte z97x-ud5h (F8 Bios)
* Processor: Intel Core i7-4790K
* TP-LINK Archer T8E AC1750 (not using LAN)
* Samsung SSD 840 PRO SSD
* macOS Sierra (originally Yoesmite)

## What's Working
* Sleep, shutdown, and restarting works
* Have not tested USB3 yet and am using USB2 for sound
* Full graphics acceleration with the NVidia Web Drivers / Cuda Drivers
* "About this Mac" correctly reports memory and graphics.

This system is running stable for the most part. However, I had TONS of issues getting this running on Sierra, so I thought I'd put this up here to help other people out. And if anyone sees any room for improvement, let me know. I'm still in the process of tweaking this install.

## What's Not Working
* See list of issues
* iPhoto will crash your Mac. Do not open it! See list of issues for more info.

## Brief Instructions (not finished)
1. Use TonyMac's guide to create a bootable USB: https://www.tonymacx86.com/threads/unibeast-install-macos-sierra-on-any-supported-intel-based-pc.200564/
2. Switch out the Clover EFI folder with this one. Please back up Clover's default clover.plist, just in case
3. You may need to add nv_disable=1 to my config.plist, since web drivers will not be installed at first
4. Install macOS Sierra (using TonyMac's guide)

## Useful Tools
* TonyMac DSDT Library and Forums
* Unibeast: create USB Installer
* Clover: awesome bootloader. Patches / adds stuff on the fly.
* Clover Configurator: easiest way to mount EFI partitions and edit config.plist.
* Nvidia Web Drivers
* CUDA Drivers
