################################################################################
HOW TO BUILD KERNEL FOR GT-I9301I_EUR

1. How to Build
	- get Toolchain
	download and install arm-eabi-4.6 toolchain for ARM EABI.
	Extract kernel source and move into the top directory.

	$ make VARIANT_DEFCONFIG=msm8226-sec_s3ve3g_eur_defconfig msm8226-sec_defconfig
	$ make

2. Output files
	- Kernel : Kernel/arch/arm/boot/zImage
	- module : Kernel/drivers/*/*.ko

3. How to Clean
    $ make clean

4. How to make .tar binary for downloading into target.
	- change current directory to Kernel/arch/arm/boot
	- type following command
	$ tar cvf GT-I9301I_EUR.tar zImage
#################################################################################
