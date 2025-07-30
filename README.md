# KernelSU v0.9.2 & v0.9.4 for Huawei nova 3i based on EMUI9.1/HarmonyOS2.0.

**English** | [简体中文](README_CN.md)

## This project is no longer under maintenance. If you are looking for a root solution, you can try [this](https://github.com/LenseTech/android_kernel_huawei_kirin710_SukiSU-Ultra-EMUI9_HarmonyOS2)

## Features
- Provide KernelSU Root.
- Module installation support.

## Devices
- HUAWEI Nova 3i(INE-AL00) based on HarmonyOS 2.0. Feel free to test for your device. (Also works theoretically on Huawei nova 5i based on HarmonyOS 2.0).

## File description
- There are two types of kernel image:
PM：Permissive
Non-PM：Enforcing
- Non-PM image also work on EMUI9.1.0.241.

## Usage
- Make sure your device bootloader has been unlocked.
- Type in adb command line: `fastboot flash kernel "PATH\TO\YOUR\KERNEL"`.
- Type `fastboot reboot` or reset by long-press the power button.
- Install official KernelSU manager. Please download the corresponding manager according to the kernel version you choose: [v0.9.2](https://github.com/tiann/KernelSU/releases/tag/v0.9.2), [v0.9.4](https://github.com/tiann/KernelSU/releases/tag/v0.9.4). 

## Attension
- Both kernels can be used when other GSIs are installed. Tested GSIs: [Arrow OS v9.0](https://sourceforge.net/projects/arrow-os/files/arrow-9.x/GSI/27_Jan_2020/), [LineageOS 16 by altairfr](https://sourceforge.net/projects/altairfr-huawei/files/LeaOS-16.0/).
- Do NOT flash PM kernel on EMUI9. It will cause Wifi function failure.

## Known Issues
- SELinux will remain Enforcing after flash PM kernel on HarmonyOS 2.0 and EMUI9.
- Some modules are incompatible, which may cause the third-party application to fail to start normally or your phone stuck in "The phone is starting...". Try remove the module that cause exception in TWRP or remove in KernelSU's Safe Mode. Modules are located in `/data/adb/modules`
- Known incompatible module(s): [Zygisk-assistant v2.1.4](https://github.com/snake-4/Zygisk-Assistant/releases/tag/v2.1.4), [Uperf-Game-Turbo.1.42](https://github.com/yinwanxi/Uperf-Game-Turbo/releases/tag/Uperf-Game-Turbo.1.42).

## Downloads
- The kernel provides the KernelSU v0.9.2 and v0.9.4 versions. Please test the stability by yourself. At present, no obvious functional differences are found between the two versions. Both versions are incompatible with the modules mentioned above.
- [Releases](https://github.com/LenseTech/android_kernel_huawei_kirin710_KernelSU-EMUI9_HarmonyOS2/releases/tag/v20250428).

## Credits
- [KernelSU](https://github.com/tiann/KernelSU/): The powerful root tool.
- [@Coconutat](https://github.com/Coconutat/): Some kernel compilation skills.

Sorry for my poor English ;)
