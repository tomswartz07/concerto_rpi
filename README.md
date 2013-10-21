Concerto2 for Raspberry Pi
==========================
Based upon Concerto for RPi by Andrew Fryer [1]


## Introduction
This document explains how to set up a Raspberry Pi
device to act as a Concerto Client 'Player'. The goal
is to have a device that, upon startup will automatically
start a web browser and navigate to the specified Concerto
content.

This program will also automatically prevent the device
from sleeping and displaying the mouse cursor.

## Setting up the Raspberry Pi
### Pre-requisites
* Raspberry Pi Model B
* Rasbian OS

### Configuring Concerto
1. Using the provided script
2. Run ./InstallConcerto.sh
3. Follow the steps to configure the server and (optionally) a ShoutCast server
4. Reboot

### Manually configuring Concerto
1. Install software requirements
```sudo apt-get install x11-xserver-utils unclutter```

2. Configure a cron script to auto-launch a web browser
	File contents can be found in the .script file
3. (Optionally) Set up your ShoutCast server settings
4. (Optionally) Set up another cron job to reboot the device daily

[1] https://github.com/flamewave000/concerto_rpi
