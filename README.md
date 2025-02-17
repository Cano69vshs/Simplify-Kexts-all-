####################################################################
#                   Configure Kernel Extensions                    #
####################################################################

List of available kexts:

### Category: Required
```
✅ **1. Lilu** - For arbitrary kext, library, and program patching  
✅ **2. VirtualSMC** - Advanced Apple SMC emulator in the kernel  
```

### Category: VirtualSMC Plugins
```
✅ **3. SMCBatteryManager** - Manages, monitors, and reports on battery status  
❌ **4. SMCDellSensors** - Enables fan monitoring and control on Dell computers  
✅ **5. SMCLightSensor** - Allows system to utilize ambient light sensor device  
❌ **6. SMCProcessor** - Manages Intel CPU temperature sensors  
❌ **7. SMCRadeonSensors** - Provides temperature readings for AMD GPUs  
❌ **8. SMCSuperIO** - Monitoring hardware sensors and controlling fan speeds  
```

### Category: Graphics
```
❌ **9. NootRX** - The rDNA 2 dGPU support patch kext  
✅ **10. NootedRed** - The AMD Vega iGPU support kext  
❌ **11. WhateverGreen** - Various patches necessary for GPUs are pre-supported  
```

### Category: Audio
```
✅ **12. AppleALC** - Native macOS HD audio for not officially supported codecs  
```

### Category: Wi-Fi
```
❌ **13. AirportBrcmFixup** - Patches required for non-native Broadcom Wi-Fi cards  
❌ **14. AirportItlwm** - Intel Wi-Fi drivers support the native macOS Wi-Fi interface  
❌ **15. IO80211FamilyLegacy** - Enable legacy native Apple Wireless adapters  
❌ **16. IOSkywalkFamily** - Enable legacy native Apple Wireless adapters  
✅ **17. itlwm** - Intel Wi-Fi drivers. Spoofs as Ethernet and connects to Wi-Fi via Heliport  
```

### Category: Bluetooth
```
✅ **18. BlueToolFixup** - Patches Bluetooth stack to support third-party cards  
❌ **19. BrcmBluetoothInjector** - Enables the Broadcom Bluetooth on/off switch on older versions  
✅ **20. BrcmFirmwareData** - Applies PatchRAM updates for Broadcom RAMUSB based devices  
❌ **21. BrcmPatchRAM2** - Applies PatchRAM updates for Broadcom RAMUSB based devices  
✅ **22. BrcmPatchRAM3** - Applies PatchRAM updates for Broadcom RAMUSB based devices  
❌ **23. IntelBluetoothFirmware** - Uploads firmware to enable Intel Bluetooth support  
❌ **24. IntelBTPatcher** - Fixes Intel Bluetooth bugs for better connectivity  
❌ **25. IntelBluetoothInjector** - Enables the Intel Bluetooth on/off switch on older versions  
```

### Category: Ethernet
```
❌ **26. AppleIGB** - Provides support for Intel's IGB Ethernet controllers  
❌ **27. AppleIGC** - Provides support for Intel 2.5G Ethernet (i225/i226)  
❌ **28. AtherosE2200Ethernet** - Provides support for Atheros E2200 family  
❌ **29. CatalinaBCM5701Ethernet** - Provides support for Broadcom BCM57XX Ethernet series  
❌ **30. HoRNDIS** - Use the USB tethering mode of the Android phone to access the Internet  
❌ **31. IntelLucy** - Provides support for Intel X500 family  
❌ **32. IntelMausiEthernet** - Intel Ethernet LAN driver for macOS  
❌ **33. LucyRTL8125Ethernet** - Provides support for Realtek RTL8125 family  
❌ **34. NullEthernet** - Creates a Null Ethernet when no supported network hardware is present  
❌ **35. RealtekRTL8100** - Provides support for Realtek RTL8100 family  
✅ **36. RealtekRTL8111** - Provides support for Realtek RTL8111/8168 family  
```

### Category: USB
```
❌ **37. GenericUSBXHCI** - Fixes USB 3.0 issues found on some Ryzen APU-based systems  
❌ **38. XHCI-unsupported** - Enables USB 3.0 support for unsupported xHCI controllers  
```

### Category: Input
```
❌ **39. AlpsHID** - Brings native multitouch support to the Alps I2C touchpad  
✅ **40. VoodooInput** - Provides Magic Trackpad 2 software emulation for arbitrary input sources  
✅ **41. VoodooPS2Controller** - Provides support for PS/2 keyboards, trackpads, and mouse  
❌ **42. VoodooRMI** - Synaptic Trackpad kext over SMBus/I2C  
❌ **43. VoodooSMBus** - i2c-i801 + ELAN SMBus Touchpad kext  
✅ **44. VoodooI2C** - Intel I2C controller and slave device drivers  
❌ **45. VoodooI2CAtmelMXT** - A satellite kext for Atmel MXT I2C touchscreen  
❌ **46. VoodooI2CELAN** - A satellite kext for ELAN I2C touchpads  
❌ **47. VoodooI2CFTE** - A satellite kext for FTE-based touchpads  
❌ **48. VoodooI2CHID** - A satellite kext for HID I2C or ELAN1200+ input devices  
❌ **49. VoodooI2CSynaptics** - A satellite kext for Synaptics I2C touchpads  
```

### Category: Brand Specific
```
❌ **50. AsusSMC** - Supports ALS, keyboard backlight, and Fn keys on ASUS laptops  
❌ **51. BigSurface** - A fully integrated kext for all Surface-related hardware  
```

### Category: Storage
```
❌ **52. CtlnaAHCIPort** - Improves support for certain SATA controllers  
❌ **53. NVMeFix** - Addresses compatibility and performance issues with NVMe SSDs  
```

### Category: Card Reader
```
❌ **54. RealtekCardReader** - Realtek PCIe/USB-based SD card reader driver  
❌ **55. RealtekCardReaderFriend** - Makes System Information recognize your Realtek card reader  
❌ **56. Sinetek-rtsx** - Realtek PCIe-based SD card reader driver  
```

### Category: TSC Synchronization
```
❌ **57. AmdTscSync** - A modified version of VoodooTSCSync for AMD CPUs  
❌ **58. VoodooTSCSync** - A kernel extension that synchronizes the TSC on Intel CPUs  
❌ **59. CpuTscSync** - Lilu plugin for TSC sync and disabling xcpm_urgency on Intel CPUs  
✅ **60. ForgedInvariant** - The plug & play kext for syncing the TSC on AMD & Intel  
```

### Category: Extras
```
❌ **61. AMFIPass** - A replacement for amfi=0x80 boot argument  
❌ **62. ASPP-Override** - Re-enable CPU power management for Intel Sandy Bridge CPUs  
❌ **63. AppleIntelCPUPowerManagement** - Re-enable CPU power management on legacy Intel CPUs  
❌ **64. AppleIntelCPUPowerManagementClient** - Re-enable CPU power management on legacy Intel CPUs  
✅ **65. AppleMCEReporterDisabler** - Disables AppleMCEReporter.kext to prevent kernel panics  
✅ **66. BrightnessKeys** - Handler for brightness keys without DSDT patches  
❌ **67. CPUFriend** - Dynamic power management data injection (requires CPUFriendDataProvider)  
❌ **68. CpuTopologyRebuild** - Optimizes the core configuration of Intel Alder Lake CPUs+  
❌ **69. CryptexFixup** - Various patches to install Rosetta cryptex  
✅ **70. ECEnabler** - Allows reading Embedded Controller fields over 1 byte long  
❌ **71. FeatureUnlock** - Enable additional features on unsupported hardware  
❌ **72. HibernationFixup** - Fixes hibernation compatibility issues  
✅ **73. IntelMKLFixup** - Dead-simple Intel Math Kernel Library patcher for AMD CPU systems  
✅ **75. RestrictEvents** - Blocking unwanted processes and unlocking features  
❌ **76. RTCMemoryFixup** - Emulates some offsets in your CMOS (RTC) memory  
```
