Stock kernel (SWA) for Samsung Galaxy Star Duos from samsung opensource.
GT-S5282_SWA_JB_Opensource.zip

Contents of Readme_KERNEL.txt found inside the zip.
################################################################################
HOW TO BUILD KERNEL FOR GT-S5282_SWA

1. How to Build
	- get Toolchain
	download and install arm-eabi-4.4.3 toolchain for ARM EABI.
	Extract kernel source and move into the top directory.

	$ export CROSS_COMPILE=/opt/toolchains/arm-eabi-4.4.3/bin/arm-eabi-
	$ make mint-vlx-rev03_defconfig
	$ make
	
2. Output files
	- Kernel : Kernel/arch/arm/boot/zImage
	- module : Kernel/drivers/*/*.ko
	
3. How to Clean	
    $ make clean
	
4. How to make .tar binary for downloading into target.
	- change current directory to Kernel/arch/arm/boot
	- type following command
	$ tar cvf GT-S5282_SWA.tar zImage
################################################################################