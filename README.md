Build rasberrypi2 image, based on yocto branch

Supported branches
==================
sumo
thud

Build steps
===========
repo init -u git@github.com:shrkamat/raspi-manifest.git -b sumo
repo sync -j4
./poky/oe-init-build-env build-pi
bitbake rpi-basic-image
