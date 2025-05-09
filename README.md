## ASUS-ROG-MAXIMUS-Z790-HERO-RX590

🖥️The overall configuration list of my black Apple host is as follows:

| Part Type            | Part Model 
|----------------------|----------------------------------------------|
| Opencore             |  1.0.5                                       |
| Version              |  macOS Sequoia15.5                           |
| Motherboard          |  ASUS ROG MAXIMUS Z790 HERO                  |
| Hard disk            |  Coiorful CN600 2T M.2 2280 NVMe PCIe        |
| Graphics             |  AMD Radeon RX 590 8GB                       |
| CPU                  |  intel i9-14900k (24) @ 3.20GHz              |
| Memory               |  32GB (2x 16GB) Kingston FURY @ 5200MHz      |
| WiFi & Bluetooth     |  Intel AX210 / BCM94360                      |
| Audio Chipset        |  ROG SupremeFX ALC4082                       |

## Support the full range of CPU models,  i9-14900K, i9-13900K, i7-13700K, i5-13600K, etc

## Compatible macOS Versions

 Monterey (12.1-12.7X)

 Ventura (13.0-13.7X)

 Sonoma (14.0-14.7X)

 Sequoia (15.0-15.5Beta3)

## ASUS-ROG-MAXIMUS-Z790-HERO-RX590Series Motherboards MacOS 15.5 Completeness:

 CPU Normal Turbo Frequency (i5/i7/i9/etc.)

 Onboard audio is normal

 The graphics card supports HDMI/DP display output

 The front and rear 3.5 audio outputs are normal

 Sleep wake-up is normal

 WIFI and Bluetooth is in normal use

 frequency conversion is in normal use

 USB（Type-C）is in normal use

I won't talk about them one by one

Solution 1: The onboard intel AX210 Bluetooth and WIFi can be driven, and the network speed is very good, but it does not support air-car. MacOS 15 requires the HELIPORT APP to use the WIFI function

Solution 2: The onboard intel AX210 Bluetooth and WIFi can be driven, and the network speed is very good, but it does not support air-carry; MacOS 15 requires OCLP patching here using option 2

If you want to achieve the additional function of air carry, you need to buy a NVME M.2 SSD to connect to the Heiguo wireless network card

The boot can support independent graphics (RX560/570/590/5500/5600/5700/6600 and other series) by default.

## OpenCore Configuration

### ACPI

| ACPIs                    |
|--------------------------|
|  SSDT-AWAC               |
|  SSDT-RHUB               |
|  SSDT-PLUG-ALT           |
|  SSDT-EC                 |
|  SSDT-PMC                | 

### Drivers

| Driver Name     |
|-----------------|
| HfsPlus         |
| OpenCanopy      |
| OpenRuntime     |
| ResetNvramEntry |
| ToggleSipEntry  |

### SIP Off/On

 Hold down the cmd R key when macOS boots up to enter Recovery mode

 Open the terminal and enter:

      # 关闭 SIP
      
      csrutil disable
      
      csrutil authenticated-root disable
      
      # 开启 SIP

      csrutil enable
      
      csrutil authenticated-root enable
      
      # 查看 SIP 状态
      
      csrutil status
      
      csrutil authenticated-root status

### Kexts

| Kext Name                             |
|---------------------------------------|
| Lilu.kext                             |
| VirtualSMC.kext                       |
| WhateverGreen.kext                    |
| SMCProcessor.kext                     |
| SMCSuperIO.kext                       |
| AppleIGC.kext                         |
| CPUFriend.kext                        |
| CPUFriendDataProvider.kext            | 
| RestrictEvents.kext                   |
| XHCI-unsupported.kext                 |
| RadeonSensor.kext                     |
| NVMeFix.kext                          |
| FeatureUnlock.kext                    | 
| HibernationFixup.kext                 | 
| CpuTopologyRebuild.kext               | 
| USBPorts.kext                         | 
| USBWakeFixup.kext                     | 
| IO80211FamilyLegacy.kext              | 
| IOSkywalkFamily                       |
| AirportItlwm-15.5Sequoia.kext         | 
| IntelBTPatcher.kext                   | 
| IntelBluetoothFirmware.kext           |
| BlueToolFixup.kext                    |
| AMFIPass.kext                         |
| RadeonBoost.kext                      |

## 关于打赏

如果您认可我的工作，请通过打赏支持我后续的更新(自觉打赏的人真少啊，免费的东西长久不了,现已改为需要密码解压，需微信或支付宝打赏入群。打赏记得留言备注你的qq号，然后申请入群时，填写你的留言为验证答案就是，我确认后会通过你的验证的。PS:之所以设置打赏，并不是为了赚大钱，当然大家打赏的多是有一些零花钱。主要是维护更新不易，每次系统一更新，有问题的话，就要工作时间之外花时间去调试，解决问题。普通群最多500人，无门槛的入群，不够用，有些机友对无门槛进入还不珍惜，进退群很随意，不看相关说明，上来就问问题的又多。不多说了，理解不理解的，就这样吧。

|  微信                                                                                 |
|---------------------------------------------------------------------------------------|
| ![1](https://github.com/user-attachments/assets/06d87fea-0d11-4bf4-b9ed-034dc7f53d06) |
|                                                                                       |

|  支付宝                                                                               |
|---------------------------------------------------------------------------------------|
| ![1](https://github.com/user-attachments/assets/b99e75b4-69d3-450a-aae4-1a610760372d) |                                                                                  |                                                                                       |


##  若有其他问题请加Q群： 738882434
