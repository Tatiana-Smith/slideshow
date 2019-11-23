# RaspberryPi Slideshow Bash Script

A small bash script that takes JPG pictures from a USB drive and stores them in
a folder and displays them in a slideshow. 


## Installation/Setup

1. `git clone https://github.com/akilhylton/slideshow.git`
	* `sudo chmod 755 requirements.sh`
	* `./requirements.sh`

2. `mkdir ~/Desktop/pictures`

3. `cd ~/slideshow`

4. `chmod 755 slideshow`


## Accuring USB Device's UUID

1. `sudo blkid -sUUID`

2. Enter your usb device's uuid in the `UUID=` variable in the slideshow bash file.  


## Add bash script to run on RaspberryPi start up

1. `cd ~/` (Goes to home directory)

2. `sudo nano /etc/rc.local`

3. `~/slideshow/slideshow` (Copy and paste this line into rc.local file))
