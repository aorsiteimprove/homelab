# homelab

## setting up external drive
https://linuxconfig.org/howto-mount-usb-drive-in-linux

fdisk -l 
mkdir /media/elements
mount -t ntfs-3g /dev/sda1 /media/elements/

vim /etc/fstab 
UUID=30E2ED3EE2ED0944 /media/elements ntfs    defaults          0       0

