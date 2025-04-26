# KernelSU v0.9.2 for Huawei nova 3i based on EMUI9.1/HarmonyOS2.0.

**English** | [简体中文](README_CN.md)

## Features
- Provide KernelSU Root.
- Module installation support.

## Devices
- HUAWEI Nova 3i(INE-AL00) based on HarmonyOS 2.0. Feel free to test for your device. (Also works theoretically on Huawei nova 5i based on HarmonyOS 2.0).

## File description
- There are two types of kernel image: PM：Permissive; Non-PM：Enforcing.
- Non-PM image also work on EMUI9.1.0.241.

## Usage
- Make sure your device bootloader has been unlocked.
- Type in adb command line: `fastboot flash kernel "PATH\TO\YOUR\KERNEL"`.
- Type `fastboot reboot` or reset by long-press the power button.
- Only use [official KernelSU v0.9.2 manager](https://github.com/tiann/KernelSU/releases/tag/v0.9.2). Don't use other versions.

## Attension
- Both kernels can be used when other GSIs are installed. Tested GSIs: [Arrow OS v9.0](https://sourceforge.net/projects/arrow-os/files/arrow-9.x/GSI/27_Jan_2020/), [LineageOS 16 by altairfr](https://sourceforge.net/projects/altairfr-huawei/files/LeaOS-16.0/).
- Do NOT flash PM kernel on EMUI9. It will cause Wifi function failure.
- SELinux will remain Enforcing after flash PM kernel on HarmonyOS 2.0.

## Downloads
- [Releases](https://github.com/LenseTech/android_kernel_huawei_kirin710_KernelSU-EMUI9_HarmonyOS2/releases/tag/v20250422).

## Credits
- [KernelSU](https://github.com/tiann/KernelSU/): The powerful root tool.
- [@Coconutat](https://github.com/Coconutat/): Some kernel compilation skills.
