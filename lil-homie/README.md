# homelab

## initial
`apt-get update`

`apt-get install git`

## setting up external drive
https://linuxconfig.org/howto-mount-usb-drive-in-linux

`fdisk -l`

`mkdir /media/elements`

`mount -t ntfs-3g /dev/sda1 /media/elements/`

`vim /etc/fstab`

`UUID=30E2ED3EE2ED0944 /media/elements ntfs    defaults          0       0`

## install docker and docker-compose
https://docs.docker.com/install/linux/docker-ce/debian/#install-using-the-convenience-script

`curl -fsSL https://get.docker.com -o get-docker.sh`

`sudo sh get-docker.sh`

`sudo usermod -aG docker andrius`

`reboot`

`docker run hello-world`

## install docker-compose
https://dev.to/rohansawant/installing-docker-and-docker-compose-on-the-raspberry-pi-in-5-simple-steps-3mgl

`sudo apt-get install libffi-dev libssl-dev`

`sudo apt-get install -y python python-pip`

`sudo apt-get remove python-configparser`

`sudo pip install docker-compose`

## install PiVPN
https://pivpn.dev/

docker version https://github.com/giggio/docker-openvpn-arm


## todo

netdata enable lm-sensors and graph cpu temp
