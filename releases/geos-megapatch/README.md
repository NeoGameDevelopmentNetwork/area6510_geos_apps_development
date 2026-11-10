# Area6510

### GEOS MEGAPATCH 64/128

System Requirements:

* C64 / C128 (+64K VDC RAM!) PAL/NTSC
* 512Kb RAM (C=REU, GeoRAM, SuperCPU, RAMLink)
* 1351 mouse or joystick, use port #1.
* GEOS 64/128 v2.x or GEOS MegaPatch 64/128 v3.x
* GEOS Desktop (DESKTOP, TopDesk, DTopDesk, GeoDesk64, dualTop)
* A 1541/1571 floppy drive (when installing from a D64, you will need to swap the source disk) and a second drive as destination drive, or a single 1581 (if installing from a D81) as the source and destination drive.

### GEOS MEGAPATCH 64/128
This directory contains the latest release of GEOS MegaPatch. Use at your own risk!

#### About
The D81 images found here contain a setup for GEOS MegaPatch64 and MegaPatch128. There are also D64 and D71 disks available.

This is the most recent release of GEOS MegaPatch, including bug fixes and enhancements.

The current releases no longer contain TOPDESK, as TOPDESK is not part of the GEOS MegaPatch core system.
TOPDESK released with MegaPatch 2000/2003 can still be used. The same applies to the original DESKTOP from GEOS 2.x.

#### Installation
Installation on a RAM1541 drive is possible with at least 512K RAM (RAM1571 with 512K will not work, with 1Mb a RAM1581 should work). A RAM1571 with 512K will be converted to a NativeMode RAMDisk.
If the target device has less than 300K of free disk space, you should use the custom setup and install only the required system files and disc drivers.
Make sure you have a file called "DESK TOP" (C64) or "128 DESKTOP" (C128) on the boot drive. This can be either DESKTOP V2 or any version of TOPDESK.

#### Supported hardware
C64/C64C (PAL/NTSC), C128/C128D, C64 Reloaded, 1541/II, 1571, 1581, CMD FD2000, CMD F4000, CMD HD (incl. parallel cable), CMD RAMLink, CMD SuperCPU 64/128, SD2IEC, C=1351, CMD SmartMouse, Joystick, C=REU, CMD REU XL, GeoRAM, BBGRAM, CMD RAMCard, 64Net (untested since 2000/2003), TurboChameleon64, Tom+/MicroMys adapter with USB/PS2 mouse.

#### Unsupported hardware
Ultimate64 with firmware >= 1.29/1.34. From this version the TurboMode is supported: MegaPatch may not install with certain settings. If MegaPatch64 is used with the Ultimate64 and TurboMode enabled, you need the experimental SuperMouse_U64 mouse driver from the gMakeBoot/update disk and set "TurboMode=TurboEnable-bit" in the firmware.

#### Notes
* Not all desktop applications support all features of the MegaPatch disk drivers. The 2000/2003 version of TOPDESK has some known bugs (disk copy, validate, especially in native mode). Make sure to use a more recent TOPDESK release.
* SD2IEC is detected as 1541/1571/1581 without the need for file based memory read emulation (see SD2IEC manual -> "XR" command). The device address is configured automatically, except for the boot device.
* For NativeMode you must configure the SD2IEC with the correct device address (i.e. drive D: = device #11).
* Use GEOS.Editor and the "Switch DiskImage/Partition" button on the "DRIVES" page (the bottom arrow for each drive) to switch the disk images.
* The current disk image on SD2IEC cannot be saved. The next time you boot, the current disk image will remain active, no matter which disk image was active when configuration was saved in GEOS.Editor.
