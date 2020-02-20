# Manjaro-RazerConf
fix-and config fie for my setup

# HeadPhones Fix
 Create  or copy file alsa.conf in: 
 cd /etc/modprobe.d/
 then as root depmod-a ;
 modprobe -r snd-hda-intel;	
 modprobe snd-hda-intel
 reboot

