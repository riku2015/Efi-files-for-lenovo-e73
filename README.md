# Efi files for lenovo e73
 files for hackintosh lenovo thinkcentre e 73

Needed files for E73 desktop pc

Serial number removed, please use your own.

Disable hibernation:
sudo pmset -a hibernatemode 0


## Booting using clove:
be sure you boot into usb then on clover shell select right drive and enable it.
https://www.insanelymac.com/forum/topic/302041-guide-asrock-h97-pro4-yosemite-with-clover-uefi-installation/

## Howtoget sound work:
https://www.tonymacx86.com/threads/applehda-realtek-audio-guide.234732/#post-1606764

## to get timed sleep working:
modify https://www.tonymacx86.com/threads/computer-sleep-slider-bar-missing.222369/
<key>UnifiedSleepSliderPref</key>
<false/>
```
sudo spctl --master-disable
sudo mount -uw /
sudo killall Finder
```
then copy new IOPlatformPluginFamily.kext
