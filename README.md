# AllCoreBoot

AllCoreBoot is a simplified OpenCore project aimed at making the process of booting macOS on Hackintosh machines as seamless and accessible as possible. Whether you're a beginner or experienced Hackintosh enthusiast, AllCoreBoot offers an easy-to-use approach to setting up OpenCore for macOS.

## Features

- **Pre-configured OpenCore**: Set up with essential patches and drivers for common Hackintosh builds.
- **Beginner-Friendly**: Clear instructions for installation and customization.
- **Device Compatibility**: Supports a range of Intel and AMD-based hardware configurations.
- **Automatic Updates**: Regularly updated with the latest OpenCore and kext versions.
- **Simple Boot Management**: Manage macOS, Windows, and Linux boot options from a single interface.

## Getting Started

### Prerequisites

- A compatible Intel or AMD-based PC.
- A USB drive (16GB or larger).
- macOS installation files (either from macOS itself or from a Mac or Hackintosh).
- **Optional**: Access to a Mac or Hackintosh (can make the proccess slightly easier).

### Installation

**For Windows**

1. **Download the AllCoreBoot Package**: Clone or download this repository.
   ```bash
   git clone https://github.com/username/AllCoreBoot.git
2. Use The MacDownloader Tool (My version of Macrecovery from OpencorePKG) to download your preffered version of MacOS.
3. Choose the correct configuration for your system (x32, x64, Laptop, Desktop etc).
4. Format the USB Drive to device defaults.
5. Drag the EFI Folder to the USB.
6. Choose the version of Mac os to install (Full Sequioa support coming soon.)
7. Open the folder of the MacOS version of choice and drag the com.apple.recovery.boot folder to the usb.
8. Download [**GenSMBIOS**](https://github.com/corpnewt/GenSMBIOS) to generate unique SMBIOS information. Run it and select **Generate SMBIOS**, as the model select **iMacPro1,1**
9. Boot and install Mac OS.

**For Mac**
1. **Download the AllCoreBoot Package**: Clone or download this repository.
   ```bash
   git clone https://github.com/username/AllCoreBoot.git
2. Use The MacDownloader Tool (My version of Macrecovery from OpencorePKG) to download your preffered version of MacOS.
3. Choose the correct configuration for your system (x32, x64, Laptop, Desktop etc).
4. Format the USB Drive to device defaults.
5. Drag the EFI Folder to the USB.
6. Choose the version of Mac os to install (Full Sequioa support coming soon.)
7. Open the folder of the MacOS version of choice and drag the com.apple.recovery.boot folder to the usb.
8. Download [**GenSMBIOS**](https://github.com/corpnewt/GenSMBIOS) to generate unique SMBIOS information. Run it and select **Generate SMBIOS**, as the model select **iMacPro1,1**
9. Boot and install Mac OS.

Notes:
- In the folder "Kexts" there are some kexts such as Airportitlwm WHICH YOU MUST change to the one corresponding with the MacOS version you have chosen
- Reset NVRAM one time
- If you have only IGPU use -igfxvesa bootarg for easy installation
- If audio does not work for you you have to change layout-id for your audio chipset. Find your codec [**here**](https://github.com/acidanthera/applealc/wiki/supported-codecs) and try setting `alcid` in `boot-args` parameter to every layout-id values from AppleALC wiki  until you get layout-id correct for your motherboard.

## Guides
**If you have any problems with installation or booting your macOS, kernel panics or another system related issue check OC configuration guide**
**If something else isn't working properly (for example USB ports, iServices, DRM/Netflix) check Post-Install guide**
 - Creating USB installer: [**\*click\***](https://dortania.github.io/OpenCore-Install-Guide/installer-guide/)
 - OpenCore configuration: [**\*click\***](https://dortania.github.io/OpenCore-Install-Guide/ktext.html)
 - Post-Install: [**\*click\***](https://dortania.github.io/OpenCore-Post-Install/)
 - Troubleshooting: [**\*click\***](https://dortania.github.io/OpenCore-Post-Install/)
 - ACPI patching: [**\*click\***](https://dortania.github.io/Getting-Started-With-ACPI/)
 - USB mapping: [**\*click\***](https://dortania.github.io/OpenCore-Post-Install/usb/)
