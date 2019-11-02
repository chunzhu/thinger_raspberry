# thinger_raspberry
A document on Raspberry Thinger Server setup.


Download raspberry pi arm64 image @ https://ubuntu-mate.org/download/  
cd ~/Downloads  
xz -d ubuntu-mate***.img.xz  
sudo dd bs=1M if=ubuntu-mate-18.04.2-beta1-desktop-arm64+raspi3-ext4.img of=/dev/sdc conv=sync  
sudo dd bs=1M if=ubuntu-mate-18.04.2-beta1-desktop-armhf+raspi-ext4.img of=/dev/sdc conv=sync  
sudo apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv 0C49F3730359A14518585931BC711F9BA15703C6  
wget -qO - https://www.mongodb.org/static/pgp/server-4.2.asc | sudo apt-key add -  
echo "deb [ arch=amd64,arm64,armv7l ] https://repo.mongodb.org/apt/ubuntu xenial/mongodb-org/4.2 multiverse" | sudo tee /etc/apt/sources.list.d/mongodb-org-4.2.list  
sudo apt-get update  
sudo apt-get install -y mongodb-org  

https://docs.thinger.io/deployment/  

https://stackoverflow.com/questions/47731910/install-mongodb-3-2-or-higher-on-raspberry-pi-3-debian-9-stretch  
https://andyfelong.com/2019/03/mongodb-4-0-6-64-bit-on-raspberry-pi-3/  
https://itsfoss.com/ubuntu-mate-raspberry-pi/  
docker does not work, due to issues with systemd
armhf does not work with mongodb version greater than 3 as it is on 32bit.

