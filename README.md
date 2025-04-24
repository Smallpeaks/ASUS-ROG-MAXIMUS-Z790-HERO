## ASUS-ROG-MAXIMUS-Z790-HERO-RX590

🖥️The overall configuration list of my black Apple host is as follows:

| Part Type            | Part Model 
|----------------------|----------------------------------------------|
| Opencore             |  1.0.5                                       |
| Version              |  macOS Sequoia15.5Beta3                      |
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

## ASUS-ROG-MAXIMUS-Z790-HERO-RX590Series Motherboards MacOS 15.5Beta3 Completeness:

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
|  SSDT-RTCAWAC            |
|  SSDT-SBUS-MCHC          |
|  SSDT-PLUG-ALT           |
|  SSDT-EC                 |
|  SSDT-USBX               | 

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

###  若有其他问题请加Q群： 738882434
