[![status - stable](https://img.shields.io/badge/status-stable-success)](https://)
[![macOS](https://img.shields.io/badge/macOS-Big_Sur_11.7.3-orange)](https://www.apple.com/macos/big-sur/)
[![macOS](https://img.shields.io/badge/macOS-Monterey_12.6.3-purple)](https://www.apple.com/macos/monterey/)
[![macOS](https://img.shields.io/badge/macOS-Ventura_13.1-yellow)](https://www.apple.com/macos/ventura/)
[![OpenCore](https://img.shields.io/badge/OpenCore-0.8.8-blue)](https://github.com/acidanthera/OpenCorePkg)

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
- SSD: WD PC SN530
- Audio Codec: ALC255
- Ethernet Card: RTL8111
- Wifi/BT Card: RTL8821CE
- Touchpad: I2C

Tested on macOS 11.7.3 Big Sur & 12.6.1 Monterey & 13.1 Ventura

OpenCore 0.8.8

**Do NOT forget to enter your SMBIOS values in the config file.**

>This is the RELEASE version of OpenCore so you may want to change it to the DEBUG version for troubleshooting.

## Working:

* Audio (Speakers, Headphones, Headset, Built-in Microphones)
* Keyboard & Touchpad
* Ethernet
* GPU Acceleration
* SSD
* Display Brightness
* Power Management
* Sleep
* Webcam
* Battery Percentage

## Not Working:
* Wi-Fi & Bluetooth (RTL8821CE is not supported on macOS; however, you can replace it with one of the AirPort cards easily)
* HDMI (doesn't work on Ice Lake GPU's, they only support DP)
* Sound disappears on headsets after some time when internal microphone activates and enters sleep state. For now, it can be fixed by unplugging the headset & plugging it back in. This only happens when the laptop wakes up after sleep.


## Notes

* Headset mic doesn't work OOB, you can use ALCPlugFix-Swift to send [appropriate verbs](https://github.com/torvalds/linux/blob/d07f6ca923ea0927a1024dfccafc5b53b61cfecc/sound/pci/hda/patch_realtek.c#L5026) in order to use it.
* If you want to use ComboJack, VerbStub is already in this EFI so just activate it in config.plist and run ComboJack_Installer/install.sh in terminal after you install macOS.

