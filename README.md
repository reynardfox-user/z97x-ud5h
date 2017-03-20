# Fractal Design Hackintosh
Working Clover configuration for z97x-ud5h, i7-4790K, GTX 760

## System Specs
* Motherboard: Gigabyte z97x-ud5h (F8 Bios)
* Processor: Intel Core i7-4790K
* macOS Sierra (originally Yoesmite)

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