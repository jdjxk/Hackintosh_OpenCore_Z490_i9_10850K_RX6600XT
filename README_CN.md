## [English README](https://github.com/jdjxk/Hackintosh_OpenCore_Intel_i5_10600KF_MSI_Z490_S01_GIGABYTE_RX5500XT_4G/blob/main/README.md)

# 列表清单

| 硬件   | 型号                                          |
| ------ | --------------------------------------------- |
| 主板   | 微星 Z490-S01                                 |
| 处理器 | 英特尔 酷睿 i5-10600KF                        |
| 内存   | 英睿达 Ballistix 16GB Kit (2 x 8GB) DDR4-3600 |
| 固态   | 英特尔 傲腾 900P 280GB                        |
| 显卡   | 技嘉 RX 5500 XT OC 4G                         |
| 无线   | 奋威 T919                                     |
| 网卡   | 英特尔 I219-V                                 |
| 声卡   | 瑞昱 ALC892                                   |

| 软件     | 版本          |
| -------- | ------------- |
| SMBIOS   | MacPro7,1     |
| OpenCore | 0.7.5         |
| macOS    | Monterey 12.0 |

# BIOS 设置

Settings\Advanced\Wake Up Event Setup\Resume By USB Device **[Disabled] -> [Enabled]**

Settings\Advanced\D.T.M **[Disabled] -> [Enabled]**

Settings\Advanced\Power Management Setup\ErP Ready **[Disabled] -> [Enabled]**

# 已知问题

[NVMeFix.kext](https://github.com/acidanthera/NVMeFix) 在 傲腾 900P 上可能导致随机出现的启动问题。

> *不使用它似乎可以正常运行。*

# 注意事项

无线网和蓝牙功能需要以下文件 [AirportBrcmFixup](https://github.com/acidanthera/AirportBrcmFixup)/[BrcmPatchRAM](https://github.com/acidanthera/BrcmPatchRAM)/[itlwm](https://github.com/OpenIntelWireless/itlwm)/[IntelBluetoothFirmware](https://github.com/OpenIntelWireless/IntelBluetoothFirmware) 。

> *在 Monterey 下需要使用 [BlueToolFixup.kext](https://github.com/acidanthera/BrcmPatchRAM) 来解决蓝牙问题。* 

如果 USB 定制不合适，请在 Windows 环境下使用 [USBToolBox](https://github.com/USBToolBox/tool) 来定制您自己的 USBMap.kext 。

