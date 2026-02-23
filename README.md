# CyberEXS GRUB Theme 🚀

A futuristic cyberpunk-style theme for the GRUB bootloader, originally created by [HenriqueLopes42](https://github.com/HenriqueLopes42/themeGrub.CyberEXS).

![CyberEXS Theme Preview](background.png)

## 📋 Table of Contents
- [Description](#description)
- [Prerequisites](#prerequisites)
- [Installation Guide](#installation-guide)
- [Uninstalling the Theme](#Uninstallation)
- [Credits](#credits)

## 🎯 Description

This theme transforms your Ubuntu GRUB boot menu into a cyberpunk-inspired interface with:
- Custom terminal-style graphics
- Cyberpunk color scheme (greens, cyans, and purples)
- Multiple font sizes for better readability
- Custom selection indicators

## 🔧 Prerequisites

Before installing, make sure you have:
- **Ubuntu** (or any Debian-based Linux distribution)
- **Administrator access** (sudo privileges)
- **Internet connection** (for downloading the theme)
- **Git** (for easy installation)

## 📥 Installation Guide

### 1. Clone the Repository
```bash
git clone https://github.com/YOUR_USERNAME/themeGrub.CyberEXS.git
```
### 2. Copy the Theme to GRUB's Themes Directory
```bash
sudo mkdir -p /boot/grub/themes
sudo cp -r themeGrub.CyberEXS /boot/grub/themes/CyberEXS
```
### 3. Edit the GRUB Configuration File
Open the GRUB default configuration file with a text editor:
```bash
sudo nano /etc/default/grub
```
Find the line that starts with #GRUB_THEME= (or add it if it doesn't exist) and change it to:
```text
GRUB_THEME="/boot/grub/themes/CyberEXS/theme.txt"
```
Make sure to remove the # at the beginning of the line if it is commented out.

### 4. Update GRUB
```bash
sudo update-grub
```
For Fedora / RHEL-based distros:
```bash
sudo grub2-mkconfig -o /boot/grub2/grub.cfg
```
### 5. Reboot
```bash
sudo reboot
```

## Uninstallation
 1.Remove the theme folder:
```bash
sudo rm -rf /boot/grub/themes/CyberEXS
```
2.Edit the GRUB config file and remove or comment out the GRUB_THEME line:
```bash
sudo nano /etc/default/grub
```
3.Update GRUB:
```bash
sudo update-grub
```

## Credits
Original Author: [HenriqueLopes42](https://github.com/HenriqueLopes42/themeGrub.CyberEXS)

Original Repository: [https://github.com/HenriqueLopes42/themeGrub.CyberEXS]
