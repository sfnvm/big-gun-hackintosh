# About
- Hackintosh installation setup.

# Specs
| Component   | Model                                                      |
| ----------- |:----------------------------------------------------------:|
| CPU         | Intel Core i7 10700                                        |
| Mainboard   | MSI MAG B460M Mortar                                       |
| RAM         | ADATA XPG Spectrix D41 (8GB x 2) bus 3000Mhz               |
| SSD-1       | SAMSUNG M2-PCIe 512GB Samsung PM981a NVMe 2280             |
| SSD-2       | Crucial P5 250GB NVMe 3D-NAND M.2 PCIe Gen3 x4 CT250P5SSD8 |
| PSU         | Xigmatek 600W                                              |

# Packages Version
- ***Base***
  - [OpenCorePkg](https://github.com/acidanthera/OpenCorePkg/releases/) *version 0.6.5*
    - Remove everything except
      ```
      .
      +-- Bootstrap
      |   +-- **
      +-- Drivers
      |   +-- OpenRuntime.efi
      +-- Tools
      |   +-- OpenShell.efi
      +-- OpenCore.efi
      ```
    - more required
        - [HfsPlus.efi](https://github.com/acidanthera/OcBinaryData/blob/master/Drivers/HfsPlus.efi)
      ```
      .
      +-- Drivers
      |   +-- HfsPlus.efi
      ```
- ***Must have***
  - [VirtualSMC](https://github.com/acidanthera/VirtualSMC/releases) *version 1.1.9*
  - [Lilu](https://github.com/acidanthera/Lilu/releases) *version 1.5.0*
  - [WhateverGreen](https://github.com/acidanthera/WhateverGreen/releases) *version 1.4.6*
  - [AppleALC](https://github.com/acidanthera/AppleALC/releases) *version 1.5.6*
  - [LucyRTL8125Ethernet](https://www.insanelymac.com/forum/files/file/1004-lucyrtl8125ethernet/) *version 1.0.0*
- ***Optionally***
  - [NVMeFix](https://github.com/acidanthera/NVMeFix/releases) *version 1.0.5*


# Resource
- [OpenCore Install Guide](https://dortania.github.io/OpenCore-Install-Guide/)

# Ultilities
- [ProperTree](https://github.com/corpnewt/ProperTree)
  - Edit .plist configuration file.
- [GenSMBIOS](https://github.com/corpnewt/GenSMBIOS)
  - Generate UUID key, mobo serial, ...
- [MountEFI](https://github.com/corpnewt/MountEFI)
  - Mount EFI partition.
- [gibMacOS](https://github.com/corpnewt/gibMacOS)
  - Download MacOS directly from Apple.