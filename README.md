# openwrt4vmware
can't remember so put here




mkdir openwrt
cd openwrt
wget https://downloads.openwrt.org/releases/19.07.1/targets/x86/64/openwrt-19.07.1-x86-64-combined-ext4.img.gz
gunzip openwrt-19.07.1-x86-64-combined-ext4.img.gz
apt-get install qemu-utils
qemu-img connect -f raw -O vmdk openwrt-19.07.1-x86-64-combined-ext4.img openwrt-19.07.1-x86-64-combined-ext4.vmdk
