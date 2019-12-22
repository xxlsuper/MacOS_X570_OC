MacOS for ASUS x570-PRO and Ryzen 7 3800X
Tested with macOS Catalina 10.15.2. All iCloud services are fully functional, but flush a new SMBIOS if you decide to use this. Rather than compiling directly from source, this configuration uses 0.5.2 - later versions have not been tested.
What is OpenCore?

OpenCore is an open-source bootloader, designed to be an alternative to Clover. OpenCore aims to resolve the constraints and issues imposed by Clover by providing a more versatile and modular system. While OpenCore is primarily designed for Hackintosh systems, it can be used in any scenario where an emulated EFI is needed. Please remember that OpenCore is still new and currently in beta. Unless you want to be on the bleeding edge of Hackintosh development or are planning on contributing to the project, you probably don't want to migrate if you have a stable system currently.

(Taken from the OpenCore Vanilla Desktop Guide)
System Specifications

    Motherboard: Asus PRO X570
        Networking: Intel I211-AT
        Audio Codec: Realtec S1220A
        Wireless: none

    CPU: AMD Ryzen 7 3800X

    GPU: Sapphire Nitro+ Radeon RX 580 8GB
        Using a Navi GPU? Add this boot flag: agdpmod=pikera

BIOS Settings

For best results, load optimised defaults - BIOS Version 2801 (24/09/2019)

    SVM Mode -> Disabled (Can be enabled post-install)
    SATA Mode -> AHCI
    IOMMU -> Disabled
    XHCI Hand-off -> Enabled
    Boot\CSM -> Disabled
    Secure Boot -> Other OS

Ryzen G CPU? Disabling CPB can help reduce audio issues.

    Core Performance Boost -> Disabled

## Guides & Links

#### Guides
- [OpenCore Vanilla Desktop Guide](https://khronokernel-2.gitbook.io/opencore-vanilla-desktop-guide/)
- [Catalina GPU Guide](https://khronokernel-3.gitbook.io/catalina-gpu-buyers-guide/)

#### Links

- [OpenCorePkg](https://github.com/acidanthera/OpenCorePkg)
- [OpenCore Changelog](https://github.com/acidanthera/OpenCorePkg/blob/master/Changelog.md)
- [Kext Repo](https://1drv.ms/f/s!AiP7m5LaOED-m-J8-MLJGnOgAqnjGw)
- [CPU Name](https://github.com/corpnewt/CPU-Name)
