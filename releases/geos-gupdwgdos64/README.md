# Area6510

### GUPDWGDOS64
gUpdWGDOS64 is a small utility to download and install GDOS64 using a WiC64 and original GEOS 2.0 (C=REU) or GEOS 2.0r (GeoRAM).
Therefore it will download GEOSConf64 first to setup a RAM1581 disk. Optional it will download geoDiskSlct64 to create or swap disk images on SD2IEC devices.


#### USAGE
##### Prerequisites:

1.	Make sure you know how to use GEOS. If not, read the BASICs section of the HowTo:

	https://bitbucket.org/mkgit64/area6510/raw/master/doc/geos-install/GEOS-HowTo.pdf

2.	Ensure that a WiC64 is connected and ready to download files.

3.	Make sure you have a RAM expansion connected, C=REU and/or GeoRAM are supported.

4.	Needed to create a boot disk: SD2IEC drive with D81 disk images or C=1581 disk drive with a blank disk.

##### WARNING!
If you are using a CMD SuperCPU or TurboChameleon64 you must set the CPU clock to 1 MHz mode! The original GEOS might not work well with a higher CPU clock.

##### Start GEOS64:

1.	Run GEOS64 with at least 2Mb RAM expansion. GEOS does not need to detect all of the RAM, it just needs to be enough to install a RAM1541 drive (512Kb). 	GEOS 2.0 or 2.0R should work.

2.	Configure drive B: as a RAM1541 disk drive.

3.	Optional: Copy "DESK TOP" to drive B: and close drive A:

4.	Insert the gUpdWGDOS64 disk into drive A:. Open drive A:.

5.	Optional: Copy "DESK TOP" from drive B: to drive A:

6.	Open drive A:. Run "WGetConf64". This will download GEOSCONF64 to drive B:, the existing content of drive B: will be destroyed!

7.	Run GEOSCONF64RH+ (GeoRAM) or GEOSCONF64H+ (C=REU), these are the recommended versions with support up to four drives and CMD HD devices.

8.	Configure at least one drive as RAM1581:
	Drive B: if you have a 1581 disk drive configured as drive C:
	or
	Drive D: / C: to download to drive D: and install to drive C: or if you want to download the SD2IEC helper tool (see next step).
	(Note: Drive D: will be removed during update with 2Mb RAM)
	or
	Drive B: / C: to download to drive B: and install to drive C:
	You can configure a SD2IEC or C=1581 drive later after GDOS64 has been installed to create a boot disk for daily use.

9.	Optional: Run "WGetDisk64". This will download GEODISKSLCT64 to drive B:. Existing content of RAM1541 drive B: will be destroyed!
	Only needed if you want to install GDOS64 to a CMD partition or SD2IEC disk drive and you need to select a new target disk.
	Note: On SD2IEC drives you can also create new disk Images!

10.	Run GD.GETUPDATE.DE (german) or GD.GETUPDATE.EN (english).
	This will download and install the GDOS64 update.

11.	The SETUP will analyze the archive which can take several minutes. If the archive is checked the SETUP will continue. Otherwise you will get an error message.
