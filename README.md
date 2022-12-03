# OpenCore EFI Folder for Acer Aspire 3 A315-56-327T

Tested on macOS 11.7.1 Big Sur

OpenCore 0.8.6

**Do NOT forget to enter your SMBIOS values in the config file.**

Working:

* Audio (Headphones, Headset with no mic support, Built-in Microphones)
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

>This is the RELEASE version of OpenCore so you may want to change it to the DEBUG version for troubleshooting.

>It includes custom AppleALC with new layout for this laptop (layout-id=69) so don't upgrade AppleALC.kext when a new update drops. I'll make a pull request soon to get my layout added to the AppleALC repo.

**ComboJack (https://github.com/hackintosh-stuff/ComboJack) IS REQUIRED TO GET SOUND FROM HEADPHONES & HEADSET AFTER SLEEP.**
>Its kexts are already in this EFI so just run ComboJack_Installer/install.sh in terminal after you install macOS.
