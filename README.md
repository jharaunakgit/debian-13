# Debian 13 “Trixie” Installation Steps

## 1 Prepare for Installation
Download the Debian 13 “Trixie” ISO from the official [Debian website](https://www.debian.org/). Select the appropriate ISO for your computer. 
You can go for the full DVD version or the netinst version of the ISO.

## 2 Audience & Scope

### 2.1 Who this is for
This guide is intended for system administrators or users familiar with basic system hardware BIOS/UEFI setup, who wish to install Debian 13.

### 2.2 What this covers
* Downloading and verifying the Debian 13 installation file 
* Creating a bootable USB installation drive
* Booting the installer
* Basic installation: partitioning, user setup, software selection
* First boot and initial configuration

## 3 Prerequisites

### 3.1 Hardware requirements(bare minimum)
For a typical desktop installation:
* Minimum 2GB RAM  
* At least 20 GB of storage
* UEFI firmware recommended; Secure Boot optional

### 3.2 Download media
* Visit the Debian download page and select the appropriate image for your architecture.
* Verify the download ISO’s checksum and optionally its GPG signature to ensure integrity. 

### 3.3 Bootable USB drive
* Prepare a USB disk (8GB or higher) to serve as installation media. 
* On Windows/Mac/Linux, Rufus/ Balena Etcher may be used.  

## 4 Installation Media
### 4.1 Create a Bootable USB Drive

Download and install Rufus or Balena Etcher according to your requirements and platform. 

### 4.2 Writing the ISO to USB

* Insert the USB stick (8 GB or larger).
* Open your chosen tool (Rufus, Balena Etcher)
* Select the downloaded ISO and choose the USB device as the target.
* Start the write process and then eject the drive once the process is completed.

### 4.3 Verifying bootability

* Reboot your system and enter the firmware (BIOS/UEFI) boot menu (typically by pressing F2/F10/Esc/F12).
* Select the USB drive.
* If you see the “Debian” installer menu, you are ready to proceed.

## 5 Installation Process

### 5.1 Start the Installer
* Choose the appropriate location and language.
* Choose the Keyboard layout.

### 5.2 Configuration
* The installer will get you going once a network setting is detected. You may need to enter the hostname, domain name, and password.

### 5.3 Clock
* The installer will get you going once the clock setting is completed. You can select the region for the clock.

### 5.4 Partitioning
Now, the option to select the mode of partitioning will show four options. You can select the first option, ***Guided - Use entire disk***. Now, the Debian setup will automatically create the partitions. 
* Select "**All files in one partition**". 
* Finally, select "**Finish Partitioning and write changes to disk**" and click **Continue**.
* One final confirmation dialog will appear, which will ask you to select **Yes** or **No**.

### 5.5 Base System
Now, you need to install the base system. It will be done by the installer after it downloads the core packages.

### 5.6 Network Mirror
You may be asked to select the option for Network Mirror. Here, you may select **Yes** and choose  an appropriate mirror.

### 5.7 Software selection
Select a desktop environment for your Debian installation. You can select a Debian desktop installation along with standard system utilities and your favorite environment. 

### 5.8 Install the Bootloader (GRUB) 
The installer will prompt you to install the bootloader.

### 5.9 User Account
Now, you need to select the User account and password for your system. 

## 6 Finish the Installation
* Finally, you need to reboot the computer.
* You can eject the USB once you see the prompt on the screen.

## 7 Boot into Debian
* Now, the system will boot for the first time into Debian.
* Finally, you will be asked for the user's password. 
