# Manjaro-RazerConf
fix-and config fie for my setup
## audio HeadPhones setup
-- cd /etc/modprobe.d
--nano alsa.conf
##add this line to the file 
options snd-hda-intel model=alc298-spk-volume
## then as root depmod-a ;
## modprobe -r snd-hda-intel;	
## modprobe snd-hda-intel
#reboot

