# Area6510

# GEOS MEGAPATCH 64/128 - KERNAL DRIVERS
Released: 2025/05/30 20:00
Version : V3.3r11

### KERNAL DRIVERS
This a testing release of the new kernal mode
disk drivers. These drivers do not make use of
the GEOS fast loader, instead they are using the
default kernal routines to access the disk.

These drivers will be really slow but can be
used for drives that do not support the GEOS
TurboDOS. Right now these drives must at least
support either a real ROM or must emulate the
ROM like an SD2IEC using the "M-R emulation".
