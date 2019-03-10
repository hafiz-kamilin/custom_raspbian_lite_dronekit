# Raspbian 4.14 Lite with pre-configured DroneKit-Python API

## Introduction

<p align = "center">
  <img src = "https://raw.githubusercontent.com/hafiz-kamilin/raspbian_4.14_lite_dronekit/master/00_readme_img/1.png" width = "878" height = "320"/>
</p>

A custom made Raspbian Lite (kernel version 4.14) pre-configured with DroneKit-Python API development environment. Do note that at the current time of making, DroneKit-Python API only supported on Python 2. Thus, this custom Raspbian Lite release will be rendered obsolete and porting the user code from Python 2 to Python 3 would be necessary when Python 2 reach it end of life (EOL).

## Installing custom Raspbian Lite

1. Download the custom Raspbian Lite image at [here](https://github.com/hafiz-kamilin/raspbian_4.14_lite_dronekit/releases/download/1.0/dronekit_basic_05.12.2018.pi_raspberry.7z) (alternatively you can access the download page from the [Release](https://github.com/hafiz-kamilin/raspbian_4.14_lite_dronekit/releases) page).
2. Install [Win32 Disk Imager](https://sourceforge.net/projects/win32diskimager/) on a Windows PC and write the image on a blank SD card to be inserted inside Raspberry Pi 3 model B.
3. Install [Advanced IP Scanner](https://www.advanced-ip-scanner.com/) on Windows PC to find the Raspberry Pi IP address and use [Bitvise SSH Client](https://www.bitvise.com/ssh-client-download) to establish the Secure Shell (SSH) connection between Windows PC and Raspberry Pi.
4. Execute ```sudo apt update && sudo apt dist-upgrade``` to update the Raspbian Lite to the current release.
5. **OPTIONAL** Update all the Python 2 packages (highly discouraged if you don't know what you're doing).

## Note

Raspbian Lite login credential
- Username: pi
- Password: raspberry

**Don't forget to change the Raspbian Lite login credential via ```sudo raspi-config```.**
