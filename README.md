# Specification

| Hardware      | Model                                          |
| ------------- | ---------------------------------------------- |
| Motherboard   | MSI Z490-S01                                   |
| CPU           | Intel Core i5-10600KF                          |
| Memory        | Crucial Ballistix 16GB Kit (2 x 8GB) DDR4-3600 |
| SSD           | Intel Optane SSD 900P 280GB                    |
| Graphics Card | Gigabyte Radeon RX 5500 XT OC 4G               |
| Network       | Intel I219-V                                   |
| Audio         | Realtek ALC892                                 |

| Software | Version       |
| -------- | ------------- |
| SMBIOS   | MacPro7,1     |
| OpenCore | 0.7.5         |
| macOS    | Monterey 12.0 |

# BIOS Settings

Settings\Advanced\Wake Up Event Setup\Resume By USB Device **[Disabled] -> [Enabled]**

Settings\Advanced\D.T.M **[Disabled] -> [Enabled]**

Settings\Advanced\Power Management Setup\ErP Ready **[Disabled] -> [Enabled]**

# Known Issues

**NVMeFix.kext** might cause booting problems randomly on Intel 900P.

> *Everything seems to be working properly without it.*

# Notice

[AirportBrcmFixup](https://github.com/acidanthera/AirportBrcmFixup)/[BrcmPatchRAM](https://github.com/acidanthera/BrcmPatchRAM)/[itlwm](https://github.com/OpenIntelWireless/itlwm)/[IntelBluetoothFirmware](https://github.com/OpenIntelWireless/IntelBluetoothFirmware) are required for Wireless and Bluetooth.

> *Use [BlueToolFixup.kext](https://github.com/acidanthera/BrcmPatchRAM) to solve Bluetooth problems in Monterey.* 

Please use [USBToolBox](https://github.com/USBToolBox/tool) in Windows environment to custom your own USBMap.kext if it's not suitable for you.
