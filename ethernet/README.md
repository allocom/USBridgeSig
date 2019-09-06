# USBridgeSig


Allo Introducing new Model USBridgeSig:

USBridgeSig is with RaspberryPi CM3+ Lite Module. The CM3+ Compute Module contains the guts of a Raspberry Pi 3 Model B+ (the BCM2837 processor and 1GB RAM)

Interfaces : 3 x USB 2.0 Host ports, HDMI , 1 Gigabit Ethernet Port (AX88179)

MicroSD card for OS (8GB or above) , Power input - 5V/3A


******************************************************

USBridgeSig having ASIX AX88179 Gigabit Etherenet Port. Asix Driver need to update  for USB audio streaming applications.

Updated Files are ax88179_178a.c , ax88179_178a.h and copy to linux source tree for compilation.

./Linux/drivers/net/usb/ax88179_178a.c
./Linux/drivers/net/usb/ax88179_178a.h

https://raw.githubusercontent.com/allocom/USBridgeSig/master/ethernet/ax88179.tar

on linux 

wget https://raw.githubusercontent.com/allocom/USBridgeSig/master/ethernet/ax88179.tar


**************
updated version check using modinfo : run below command , result will be v0.1.4

modinfo ax88179_178a | grep version

version:        v0.1.4


info : Pull Request  submited on Raspberrypi Linux kernel repository

https://github.com/raspberrypi/linux/pull/2999
