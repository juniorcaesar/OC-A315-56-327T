# OpenCore EFI Folder for Acer Aspire 3 A315-56-327T

![Big Sur](https://raw.githubusercontent.com/juniorcaesar/OC-A315-56-327T/main/Screenshots/SCR-20221203-jf4.jpeg)
<p align="center">
macOS Big Sur 11.7.1
</p>

![Monterey](https://raw.githubusercontent.com/juniorcaesar/OC-A315-56-327T/main/Screenshots/SCR-20221210-ih7.jpeg)
<p align="center">
macOS Monterey 12.6.1
</p>

- CPU: Intel Core i3-1005G1
- GPU: Intel UHD Graphics G1
- RAM: 8 GB 2666MHz / Dual Channel
- SSD: WD Green SN530
- Audio Codec: ALC255
- Ethernet Card: RTL8111
- Wifi/BT Card: RTL8821CE
- Touchpad: I2C

Tested on macOS 11.7.1 Big Sur & 12.6.1 Monterey

OpenCore 0.8.6

**Do NOT forget to enter your SMBIOS values in the config file.**

Working:

* Audio (Headphones, Headset, Built-in Microphones)
* Keyboard & Touchpad
* Ethernet
* GPU Acceleration
* SSD
* Display Brightness
* Power Management
* Sleep
* Webcam
* Battery Percentage
* Boot Chime

Not Working:
* Wi-Fi & Bluetooth (RTL8821CE is not supported on macOS)
* HDMI (doesn't work on Ice Lake GPU's, they only support DP)
* Headset mic doesn't work OOB, you can use ALCPlugFix-Swift to send [appropriate verbs](https://github.com/torvalds/linux/blob/d07f6ca923ea0927a1024dfccafc5b53b61cfecc/sound/pci/hda/patch_realtek.c#L5026) in order to use it.

>This is the RELEASE version of OpenCore so you may want to change it to the DEBUG version for troubleshooting.

* This EFI includes custom AppleALC with new layout for this laptop (layout-id=69) so don't upgrade AppleALC.kext when a new update drops. I'll make a pull request soon to get my layout added to the AppleALC repo (when i properly fix inputs/outputs, i'm working on this for 4 weeks :( ).

* If you need headset mic, ComboJack is confirmed to work on Big Sur. However, it makes an activation & deactivation noise (loud pop) through headphones when it is used on Monterey.
>VerbStub is already in this EFI so just activate it in config.plist and run ComboJack_Installer/install.sh in terminal after you install macOS.

