[![status - stable](https://img.shields.io/badge/status-stable-success)](https://)
[![macOS](https://img.shields.io/badge/macOS-Big_Sur_11.7.4-orange)](https://www.apple.com/macos/big-sur/)
[![macOS](https://img.shields.io/badge/macOS-Monterey_12.6.1-purple)](https://www.apple.com/macos/monterey/)
[![macOS](https://img.shields.io/badge/macOS-Ventura_13.1-yellow)](https://www.apple.com/macos/ventura/)
[![OpenCore](https://img.shields.io/badge/OpenCore-0.8.9-blue)](https://github.com/acidanthera/OpenCorePkg)

![Acer Aspire 3 A315-56](https://raw.githubusercontent.com/juniorcaesar/OC-A315-56-327T/main/Screenshots/aspire.png)

- CPU: Intel Core i3-1005G1
- GPU: Intel UHD Graphics G1
- RAM: 8 GB 2666MHz / Dual Channel
- SSD: WD PC SN530
- Audio Codec: ALC255
- Ethernet Card: RTL8111
- Wifi/BT Card: RTL8821CE
- Touchpad: I2C

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
* Wi-Fi & Bluetooth (RTL8821CE is not supported on macOS; however, you can replace it with one of the supported cards easily)
* HDMI (doesn't work on Ice Lake GPU's, they only support DP)
