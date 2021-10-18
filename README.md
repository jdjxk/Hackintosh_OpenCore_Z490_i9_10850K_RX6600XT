## [中文说明](https://github.com/jdjxk/Hackintosh_OpenCore_Intel_i5_10600KF_MSI_Z490_S01_GIGABYTE_RX5500XT_4G/blob/main/README_CN.md)

# Specification

| Hardware      | Model                                          |
| ------------- | ---------------------------------------------- |
| Motherboard   | MSI Z490-S01                                   |
| CPU           | Intel Core i5-10600KF                          |
| Memory        | Crucial Ballistix 16GB Kit (2 x 8GB) DDR4-3600 |
| SSD           | Intel Optane 900P 280GB                        |
| Graphics Card | Gigabyte RX 5500 XT OC 4G                      |
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

[NVMeFix.kext](https://github.com/acidanthera/NVMeFix) might cause booting problems randomly on Intel 900P.

> *Everything seems to be working properly without it.*

# Notice

[AirportBrcmFixup](https://github.com/acidanthera/AirportBrcmFixup)/[BrcmPatchRAM](https://github.com/acidanthera/BrcmPatchRAM)/[itlwm](https://github.com/OpenIntelWireless/itlwm)/[IntelBluetoothFirmware](https://github.com/OpenIntelWireless/IntelBluetoothFirmware) are required for Wireless and Bluetooth.

> *Use [BlueToolFixup.kext](https://github.com/acidanthera/BrcmPatchRAM) to solve Bluetooth problems in Monterey.* 

Please use [USBToolBox](https://github.com/USBToolBox/tool) in Windows environment to custom your own USBMap.kext if not suitable.

