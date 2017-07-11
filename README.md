# About
This is a source code of uBoot for UAVX board.

# Download source code
    git clone https://github.com/Radoslaw-Przybysz/uboot.git
    cd uboot

# Install & select cross compiler

### If you do not have any compiler installed (or you are not sure)
    sudo apt-get install gcc-arm-linux-gnueabihf
    export CROSS_COMPILE=arm-linux-gnueabihf-
	
	or if not
	
	git clone https://github.com/Radoslaw-Przybysz/gcc-arm-linux-gnueabihf-4.7
	export CROSS_COMPILE=$PWD/gcc-arm-linux-gnueabihf-4.7/bin/arm-linux-gnueabihf-

# Setup Architecture
    export ARCH=arm

# Build 
Here are instructions how to compile the source code

    make distclean
    make mx6quavx_config
    make
