# thinger_raspberry
A document on Raspberry Thinger Server setup.


Download raspberry pi arm64 image @ https://ubuntu-mate.org/download/
cd ~/Downloads
xz -d ubuntu-mate***.img.xz
sudo dd bs=1M if=ubuntu-mate-18.04.2-beta1-desktop-arm64+raspi3-ext4.img of=/dev/sdc conv=sync
sudo dd bs=1M if=ubuntu-mate-18.04.2-beta1-desktop-armhf+raspi-ext4.img of=/dev/sdc conv=sync

https://docs.thinger.io/deployment/

https://stackoverflow.com/questions/47731910/install-mongodb-3-2-or-higher-on-raspberry-pi-3-debian-9-stretch
https://andyfelong.com/2019/03/mongodb-4-0-6-64-bit-on-raspberry-pi-3/
https://itsfoss.com/ubuntu-mate-raspberry-pi/
