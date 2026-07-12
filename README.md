# The Weien Kernel Project #

# info

This is The Weien Kernel Project side line for RedmiNote10Pro(Chopin)MIUI14 Android13 Root Use ReSukiSU with susfs And KVM
这是TheWeienKernelProject支线版本给note10pro chopin miui14 安卓13 集成杂鱼 susfs kvm

# How Install 安装指南
1.下载releases提供的ak3包 Install AnyKernel3
2.在Recovery里面卡刷刷入 Recovery sideload 
3.等待启动   Boot Phone         

## KERNEL WARNING ##
> EFI ACPI无法使用

## U Can Build With This: 你可以这样编译 ##
```
cd android_WeienKernel_xiaomi_chopin
```
```
使用内核集成脚本 Use Kernel Setup Scripts
```
```
make vendor/chopin_defconfig vendor/addon.config
```
```
make -j$(nproc) Image | tee ~/build.log
```

| Kernel Version 内核版本 | 
|----------------|
| Linux Kernel 4.14.186 |

## kernel support
| Supported 支持 | Satus 状态 |
|---------|-------------|
| **EFI(Testing测试中)** | ✅ |
| **ACPI(Testing测试中)** | ✅ |
| **KVM** | ✅ |
| **DroidSpaces** | ✅ |
| **Kprobes** | ✅ |
| **BPF** | ✅ |
| **ResukiSU** | ✅ |
| **sufus** | ✅ |
*Testing测试中代表无法使用但已集成
