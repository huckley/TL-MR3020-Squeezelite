# TL-MR3020-Squeezelite
use TL-MR3020 with squeezelite for cheap multiroom audio

The Goal was to have a cheap multiroom audio. And a TL-MR3020 V1 was found somware.

## How to build it self
First we need to make sure the dependencies are installed (for Debian/Ubuntu):

```
sudo apt install subversion g++ zlib1g-dev build-essential git python time
sudo apt install libncurses5-dev gawk gettext unzip file libssl-dev wget
sudo apt install libelf-dev
```
or for ubuntu 18.04 or later
```
sudo apt install build-essential libncurses5-dev python unzip   
```
Get the OpenWrt source code:
```
git clone https://git.openwrt.org/openwrt/openwrt.git/
cd openwrt
git checkout lede-17.01

./scripts/feeds update -a
./scripts/feeds install -a

make menuconfig
```
