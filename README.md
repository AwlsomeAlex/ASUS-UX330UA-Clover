# macOS High Sierra + Clover Bootloader for Asus ZenBook UX330UAR
## WARNING: Unfinished and Untested
###### Last updated: 8/25/18

## Specifications:
* Model: UX330UA-AH55 (UX330UAR)
* BIOS Version: 301
* CPU: Intel Core i5-8250U
* GPU: Intel UHD Graphics 620
* RAM: 8GB LPDDR3
* Display: 1920x1080 (FHD)
* Storage: 256GB Micron M.2 SATA SSD
* Wi-Fi: Intel 802.11ac (Model Unknown)

### Warning:
Your devices specifications can be different than mine, please proceed with caution as this guide was created to work on **MY SPECIFIC DEVICE!** This should work with other UX330UAR (8th Generation i5). [If you're using a 7th Generation Core i5 check out this guide.](https://github.com/Rybo713/UX330UA-macOS)

## Working Features:
* Unknown

## Features Not Working:
* Unknown

## Pre-Installation Guide::
1. Replace Wi-FI Card with DW1560 (Recommended) or use a USB Wi-Fi Adapter (Not Recommended)
2. **WARNING: The entire disk will be deleted! Please backup data from previous OS!**
3. Change the following BIOS Options:
* **DISABLE** VT-d
* **ENABLE** Legacy USB Support
* **DISABLE** Secure Boot
* **ENABLE** Launch CSM
* Set DVMT to **64M**
* Change boot priority to **USB**

## Installation Guide:
1. Create a macOS Installation USB **(at least 16GB)**
2. Install Clover to USB (Change Install Location) then Select Customize
3. Select "Clover for UEFI booting only" and then under "UEFI Drivers" select "OsxAptioFix3Drv-64"
4. Select Install, afterwards in EFI mount replace original config.plist with provided one
5. Place provided kexts in CLOVER/kexts/other and the HFSPlus.efi in CLOVER/drivers64UEFI
6. Boot into USB on UX330UAR and Partition/Install macOS **(MAKE SURE NOTHING IS PLUGGED IN!)**

## Post-Installation Guide:
1. To Be Added

## FAQs:
* None

## Credits:
* AwlsomeAlex (UX330UAR)
* Ryan Wong (UX330UAK)
