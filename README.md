# Setting Up Raspberry Pi

**This tutorial covers how to connect Raspberry Pi to Laptop wirelessly. Share your Raspberry Pi screen on laptop screen and control it with laptop mouse and keyboard.**

**You can find the Tutorial posted [here.](https://github.com/samvidita/Connect-RaspberryPi-to-laptop-wirelessly?tab=readme-ov-file#connect-raspberry-pi-to-laptop-wirelessly)**

Step 1: Setup Raspberry Pi with a fixed IP Address for remote access. 

![WirelessSetting](doc/WirelessSetting.png)

Step 2: Set the fix IP Address for the Raspberry Pi

![WirelessDetails](doc/WirelessDetails.png)

# Install MariaDB and PHPMyAdmin on Raspberry Pi 

**You can find the Tutorial posted [here](https://raspberrytips.com/install-mariadb-raspberry-pi) or [here.](https://pimylifeup.com/raspberry-pi-mysql)**

# Install HIDdevice module in Node-Red 

**You can find the Tutorial posted [here](https://flows.nodered.org/node/@gdziuba/node-red-usbhid) and [here.](https://github.com/node-hid/node-hid#linux-notes)**

> _Note : HIDdevice is for connecting the RFID scanner to Node-Red

# Set the Admin password in Node-Red 

**You can find the Tutorial posted [here](https://discourse.nodered.org/t/password-in-node-red/50288/43?page=3) or [here.](https://discourse.nodered.org/t/node-red-security-password/10774/4)**

# Set Chromium Browser to Launch on Boot 

The easiest way to launch an application on boot is to modify the autostart file, which is used to configure applications that run when the desktop environment starts.

1. Open a terminal on your Raspberry Pi.
2. Open the autostart file for editing:

    sudo nano /etc/xdg/lxsession/LXDE-pi/autostart

3. Add the following line to the end of the file to start Chromium:

   @chromium-browser --start-fullscreen https://www.example.com

You can replace https://www.example.com with the website or local file you want to open. Remove --start-fullscreen if you don’t want it in full screen.

4. Press Ctrl + X, then Y and Enter to save and exit the file.
5. After making the changes, reboot your Raspberry Pi to see the browser launch on startup:

    sudo reboot
