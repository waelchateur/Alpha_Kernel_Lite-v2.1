How to Build

	- get one of these Toolchains for bugless compilation
	
arm-eabi-linaro-5.2
or
arm-eabi-linaro-4.8

use these make commands to start

			cd kernel
			make clean && make mrproper
			make ARCH=arm Alpha_lite_defconfig
			make ARCH=arm

Output files
	- Kernel : arch/arm/boot/zImage
	- module : drivers/*/*.ko
	
use this commande to search modules if there is :
find . -name "*.ko" -exec cp {} /home/android/modules/ \;
