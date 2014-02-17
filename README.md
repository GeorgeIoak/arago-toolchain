arago-toolchain
================

Arago Toolchain used to cross compile for AM1802

Users of ARM 9 machines
For users who are interested in ARM 9 machines (ie AM18x) then the Linaro toolchain can not be used. Instead the Arago Toolchain must be used.

Install the Arago toolchain

$ wget http://downloads.ti.com/sdoemb/sdoemb_public_sw/arago_toolchain/2011_09/exports/arago-2011.09-armv5te-linux-gnueabi-sdk.tar.bz2

$ tar -jxvf arago-2011.09-armv5te-linux-gnueabi-sdk.tar.bz2 -C $HOME

The toolchain will be installed in the arago-2011.09 directory under your $HOME directory. You can also install it in a system-wide location, just make sure to update the location in your PATH environment variable.

Host tools

Some generic development tools are required on your host Linux machine. The below commands are specific to Ubuntu Linux distribution (tested on 10.04 and 12.04 versions), please adopt to your distribution of choice accordingly.

Install development tools

$ sudo apt-get install git build-essential diffstat texinfo gawk chrpath

If you are using a 64-bit Linux, then you'd also need to install 32-bit support libraries, needed by the pre-built Linaro toolchain and other binary tools.
Install 32-bit support libraries

$ sudo apt-get install ia32-libs


It is also recommended to switch your system shell from Ubuntu's standard dash to more universal bash.
Switch shell from dash to bash
