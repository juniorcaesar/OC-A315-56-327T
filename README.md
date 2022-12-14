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
- SSD: WD Blue SN530
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

Not Working:
* Wi-Fi & Bluetooth (RTL8821CE is not supported on macOS; however, you can replace it with one of the AirPort cards easily)
* HDMI (doesn't work on Ice Lake GPU's, they only support DP)
* Headset mic doesn't work OOB, you can use ComboJack or ALCPlugFix-Swift to send [appropriate verbs](https://github.com/torvalds/linux/blob/d07f6ca923ea0927a1024dfccafc5b53b61cfecc/sound/pci/hda/patch_realtek.c#L5026) in order to use it.

>This is the RELEASE version of OpenCore so you may want to change it to the DEBUG version for troubleshooting.

* Headphones / Headsets may produce static noise when you unplug the power adapter. To solve it, put the computer into sleep mode and wake it after waiting for 4 or 5 seconds.

* If you want to use ComboJack, VerbStub is already in this EFI so just activate it in config.plist and run ComboJack_Installer/install.sh in terminal after you install macOS.

