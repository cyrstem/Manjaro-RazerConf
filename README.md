# Manjaro-RazerConf


fix-and config file for my setup

# HeadPhones Fix
 Create  or copy file alsa.conf in: 
	
 ```cd /etc/modprobe.d/
 then as root depmod-a ;
 	'modprobe -r snd-hda-intel;	
 	'modprobe snd-hda-intel
 reboot
```
# Save  packages
	pacman -Qqe >packages.txt

# Reinstall packages 
	sudo pacman -S --needed - <packages.txt
# Install Missing icons for APPS
create appname.desktop
''
move file from to
sudo mv /home/jacos/KodeLife.desktop /usr/share/applications/'
and put icons in :
'cd /usr/share/pixmaps/'

# Enable autodiscover AirPlay Client support on Arch Linux ( like on macOS )

## Step 1

Install required dependencies
```sh
pacman -S avahi pulseaudio-zeroconf
```

## Step 2

Enable and Start Avahi daemon
```sh
systemctl enable --now avahi-daemon.service
```

## Step 3

Enable the required module on Pulseaudio ( paste this at the end of `/etc/pulse/default.pa` ):
```sh
### Enable AirPlay support
load-module module-raop-discover
```

## Step 4

Restart Pulseaudio:
```sh
systemctl --user restart pulseaudio.service

```
## Step 5
removing manjaro terminal icons :
```
https://github.com/romkatv/powerlevel10k
```
