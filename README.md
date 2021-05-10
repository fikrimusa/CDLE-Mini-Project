<h1 align="justify"> Interfacing three different sensors with Raspberry Pi through different protocols, presenting the sensor data, and integrating an AI model on a dashboard. </h1>
The project used Raspberry Pi as a central control unit coupled with three different sensors that communicate different communication protocols and display all sensor data on a dashboard. To also integrate an AI model on the dashboard. 

## Walkthrough of steps to install and run the project


### Prerequisites
The project has been developed and tested using the Raspbian operating system.

### Hardware requirements
1.  Raspberry Pi 4 Model B 8GB.
2.  Ultrasonic sensor (US100).
3.  Digital intensity sensor (BH1750FVI).
4.  Temperature sensor (TMP36).
5.  RPi Approved Phidisk Class10 U1 MicroSD-64GB.
6.  MCP3008 - 8-Channel 10-Bit ADC With SPI Interface.
7.  Logitech USB camera C270 model.
8.  USB microSD Card Reader and Writer.
9.  Raspberry Pi 4 Power Switch Supply Cable USB C.
10. Soldering tools (Soldering Iron, Solder Wire, Desoldering Pump, Soldering Iron Stand, Cleaning Sponge, Tweezers, Wire Stripper/Cutter).
11. Multimeter.

### Software requirements.
1.  Raspbian operating system.
2.  Node-RED.
***

## Raspbian operating system
The installation of Raspberry Pi operating system can be done by manually or automatically. Recommended to install automatically because it saves a lot of time.
1. Installation for Raspberry Pi operating system (Manually)
+ Format SD card
+ Open file explorer, click format sd card
+ File system = FAT32 (Default).
2. Install OS Raspberry Pi (Raspbian)
+ Install BalenaEtcher.
+ Open BalenaEtcher, Select Image (Installed OS zip file), select sd card and flash.
3. Setup in Raspberry Pi - Download Raspbian (Recommended).
4. Update Raspberry Pi
+ Open terminal type "sudo apt-get update".
+ Then "sudo apt-get upgrade".
+ Reboot.
5. Installation for Raspberry Pi operating system (Automatically)
+ Install Raspberry Pi Imager
+ Format SD card
+ Choose operating system and install
***

## Node-RED
Running on Raspberry Pi. Installing and Upgrading Node-RED.

1.  Running the following command will download and run the script. If you want to review the contents of the script first, you can view it here.
bash <(curl -sL https://raw.githubusercontent.com/node-red/linux-installers/master/deb/update-nodejs-and-nodered)


2.  This script will:
+ remove the pre-packaged version of Node-RED and Node.js. if they are present.
+ install the current Node.js LTS release using the NodeSource. If it detects Node.js is already installed from NodeSource, it will ensure it is at least Node 8, but otherwise leave it alone
+ install the latest version of Node-RED using npm
+ optionally install a collection of useful Pi-specific nodes
+ setup Node-RED to run as a service and provide a set of commands to work with the service

3.  The install script for the Pi also sets it up to run as a service. This means it can run in the background and be enabled to automatically start on boot.

4.  The following commands are provided to work with the service:

+ node-red-start (this starts the Node-RED service and displays its log output. Pressing Ctrl-C or closing the window does not stop the service; it keeps running in the background)

+ node-red-stop (this stops the Node-RED service)

+ node-red-restart (this stops and restarts the Node-RED service)

+ node-red-log (this displays the log output of the service)

5.  You can also start the Node-RED service on the Raspbian Desktop by selecting the Menu -> Programming -> Node-RED menu option.
