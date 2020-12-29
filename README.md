# OpenCore EFI for MSI B550M-Pro VDH WIFI

# Specification

| **Component** | **Model** |
| ------------- | --------- |
| CPU | AMD Ryzen 3 3100 @ 3.6GHz |
| Motherboard | MSI B550M-Pro VDH WIFI |
| RAM | 8GB Corsair Vengeance LPX 3000mhz C16|
| Audio Chipset | Realtek® ALC892/ALC897 Codec |
| GPU | Radeon™ RX 480 G1 Gaming 8G |
| WiFi & Bluetooth | Intel® Dual Band Wireless-AC 3168 |
| Lan |  Realtek® 8111HN Gigabit LAN controller |
| OS Disk | Patriot 480GB SSD |
| macOS | Big Sur 11.1/ OpenCore 0.6.4 Alpha

## What works
- Audio (`alcid=28`)
- Ethernet
- USB
- Wi-Fi
- Bluetooth
- iMessage, FaceTime

## Known issues
- Airdrop and Airplay
- 3.5mm Jack microphone (haven't tested)

## Important
- Please fill out PlatformInfo -> Generic -> MLB, SystemSerialNumber and SystemUUID. For further info please visit: https://github.com/corpnewt/GenSMBIOS
- It was hard to make Ethernet work. I had to go to info.plist file inside kexy and change "OSBundleRequired" to Root. The value should be System-Root by default. It did not work with default value. So, I changed it to Root. Now works perfect. 

## Credits
- Thanx to Hackintosh & Dortania Teams for all information

