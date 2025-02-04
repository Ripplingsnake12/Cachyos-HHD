```
git clone https://github.com/Ripplingsnake12/Cachyos-HHD.git
```

# Cachyos-HHD
+ Download Cachyos Desktop edition from here-  https://cdn77.cachyos.org/ISO/desktop/250202/cachyos-desktop-linux-250202.iso
+ Burn using Etcher, Ventoy or rufus to your usb
+ You will need a dock and wired keyboard for first install.
+ Select sdboot manager, set language etc
+ Leave desktop to plasma.
+ Fill in your prefered username and password do not touch any other log in option!.
+ Once booted you will get the sddm log in screen fill in your password and select wayland session at the bottom and log in.
+ Run this
```
sudo cp -r /home/$(whoami)/Cachyos-HHD/etc /etc  /home/$(whoami)/Cachyos-HHD/usr /usr
```
+ Goto 
+ /etc/sddm.conf.d/steam-deckify.conf
+ 
+ Open the file it will look like this
+ [General]
DisplayServer=wayland
GreeterEnvironment=QT_WAYLAND_SHELL_INTEGRATION=layer-shell
[Autologin]
Relogin=true
#This is only for first boot as a file that overrides this gets created once /usr/lib/os-session-select runs
Session=gamescope-session.desktop
User= # Add your user name here, save and close

+ Run This
+ 
```
sudo pacman -S discover flatpak
sudo pacman -Rdd kwallet
sudo pacman -R inputplumber
curl -L https://github.com/hhd-dev/hhd/raw/master/install.sh | bash

```
+ Reboot you should now have Auto log in to game mode, desktop and HHD 




