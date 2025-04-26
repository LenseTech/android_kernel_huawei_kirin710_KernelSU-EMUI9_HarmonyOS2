# 适用于华为Nova 3i EMIU9.1/鸿蒙2.0底包的KernelSU v0.9.2。

## 功能
- 为华为Nova 3i提供KernelSU Root。
- 可安装模块。

## 适用设备
- 基于鸿蒙2.0的华为Nova 3i(INE-AL00)，其他同型号设备请自行测试（Nova 5i鸿蒙2.0底包理论可用）。

## 文件说明
- 压缩包内共有两种内核镜像，分别代表两种SELinux状态：
PM：宽容模式
无PM：强制执行
- 底包为EMUI9.1.0.241也可使用此内核镜像（非PM版），其他版本请自行测试。

## 使用方法
- 确保Bootloader已经解锁。
- adb命令行输入`fastboot flash kernel "你的内核路径"`。
- 使用`fastboot reboot`或长按电源键重启手机。
- 安装[官方KernelSU v0.9.2管理器](https://github.com/tiann/KernelSU/releases/tag/v0.9.2)，不要使用其他版本。

## 注意事项
- 在刷入其他GSI的情况下两种内核均可使用。已测试的GSI：[Arrow OS v9.0](https://sourceforge.net/projects/arrow-os/files/arrow-9.x/GSI/27_Jan_2020/)、[LineageOS 16 by altairfr](https://sourceforge.net/projects/altairfr-huawei/files/LeaOS-16.0/)。
- 请勿在EMUI9刷入PM内核，会导致连不上WIFI。
- 在HarmonyOS 2.0刷入PM内核后，SELinux状态仍为强制执行。

## 下载
- 请转到[发行版](https://gitee.com/lensetech/android_kernel_huawei_kirin710_-kernel-su-harmony-os2_emui9/releases/tag/v20250422)下载。

## 鸣谢
- [KernelSU](https://github.com/tiann/KernelSU/)：提供Root方案。
- [@Coconutat](https://github.com/Coconutat/)：提供内核的编译思路和技巧。