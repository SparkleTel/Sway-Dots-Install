# Sway-Dots-Install
A semi-user friendly everforest themed sway config

This script is made for linux with bash
but it should run on any UNIX-like system. Probably will not work though.
The installer will install my dots and all dependencies
the default terminal emulator on Arch is Ghostty on Debian/Ubuntu based and Fedora Suff its kitty by default this can be changed in ~/.config/sway/config.d/defaults
Distro support is limited at the moment supported distros: Debian/Ubuntu based, Arch & Arch based, Fedora and any thing similar
its also recommended that you don't have any installed WM or DE the script will NOT install a display manager I recommend 
that you use sddm to install it run:
Fedora
```
sudo dnf install sddm
```
Should be preinstalled

Debian/Ubuntu based
```
sudo apt install sddm
```
Arch
```
sudo pacman -S sddm
```
Then to enable to run on start enter the command 
```
systemctl enable sddm
```
NOTE: This will only work on distro using systemd as an init system.
If you don't want a display manager run the "Sway" command After you login in a tty

I am also working on a config for sddm that will be available in a separate repo someday


## Install
### 1. Clone The repository
You must have git install to download this script
use your systems package manager apt, pacman, dnf etc... and install the package "git"
Fedora
```
sudo dnf install git 
```
Should be preinstalled

Debian/Ubuntu based
```
sudo apt install git
```
Arch
```
sudo pacman -S git
```
After you have confirmed git is installed run: 
```
git clone https://gitlab.com/sparkletel-group/Sway-Dots-Install.git
```
### 2. Make the script executable
```
cd ./installer.sh
```
```
chmod +x ./installer.sh
```
### 3. Run the installer
Make sure to select the correct distro or the install will fail!
```
./installer.sh
```
Now Reboot 


## Defaults
File Manager: Thunar
Terminal File Manager (Arch): Yazi
Notification Daemon: Dunst
Application Launcher: Fuzzle

The display resolution by default is 1920x1080 at 100hz that can be changed in ~/.config/sway/config.d/output

Neovim with lazyvim will also be installed if you are not familiar with vim you can use micro which is a text editer that is better then nano 

