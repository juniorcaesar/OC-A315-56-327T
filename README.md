[![status - stable](https://img.shields.io/badge/status-stable-success)](https://)
[![macOS](https://img.shields.io/badge/macOS-Big_Sur_11.7.9-orange)](https://www.apple.com/macos/big-sur/)
[![macOS](https://img.shields.io/badge/macOS-Monterey_12.6.1-purple)](https://www.apple.com/macos/monterey/)
[![macOS](https://img.shields.io/badge/macOS-Ventura_13.1-yellow)](https://www.apple.com/macos/ventura/)
[![OpenCore](https://img.shields.io/badge/OpenCore-0.9.3-blue)](https://github.com/acidanthera/OpenCorePkg)

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

>Use the DEBUG version to test this EFI on your computer first. After you validate that it works without a problem, you can switch to the RELEASE version.

## Working:

* Audio (Speakers, Headphones*, Built-in Microphones)
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

## Additional Notes

**Do NOT update the VoodooI2C.kext, it breaks the physical trackpad buttons on this device.**

* You need to patch your laptop after the macOS installation in order to use headphones. Head over to Patches/Headphone Patch and read the README.md for additional info.
	- Sound may not come through headphones when the built-in microphone is activated after sleep. In that case, you can plug off & plug in the headphones to solve it.  

* Sometimes there will be a latency in registering the trackpad inputs while the laptop is connected to AC power. 
