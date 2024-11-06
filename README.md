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
- **Optional**: Access to a Mac or Hackintosh to create the installation USB.

### Installation

1. **Download the AllCoreBoot Package**: Clone or download this repository.
   ```bash
   git clone https://github.com/username/AllCoreBoot.git
3. Choose the correct configuration for your system (x32, x64, Laptop, Desktop etc).
3. Format the USB Drive to device defaults.
4. Drag the EFI Folder to the USB.
5. Choose the version of Mac os to install (Sonoma Coming soon.)
6. Open the folder of the MacOS version of choice and drag the com.apple.recovery.boot folder to the usb.
7. Boot and install Mac OS.

Note: In the folder "Kexts" there are some kexts such as Airportitlwm WHICH YOU MUST change to the one corresponding with the MacOS version you have chosen.

This bootloader was Built from an example opencore bootloader.
