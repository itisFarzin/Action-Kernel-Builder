# Build Recovery using Github Actions

## Release Notes
```
= 2024/01/14
- Adding a step to showing user inputs
- User input arranged
- Codename in the name of the flashable zip
= 2024/01/12
- The first available version is submitted.
```
-----

## Parameter Description
| Name | Description | Example |
| ------------ | -------------------- | ------------ |
| `Custom Build Title` | Set a custom build title when senfing notification to the telegram | Platina 4.19 KSU |
| `Send Notification` | Should send notification to telegram | ticked |
| `Kernel Tree` | Kernel address | https://github.com/itisFarzin/kernel_xiaomi_sdm660 |
| `Kernel Tree Branch` | Kernel branch | SW-3.2.7-KSU |
| `Phone Codename` | Use to build kernel (**CODENAME**_defconfig) and in the notifications | platina |
| `AnyKernel Url` | AnyKernel address | https://github.com/itisFarzin/AnyKernel3 |
| `AnyKernel Branch` | AnyKernel branch | platina |
| `Clang Version` | Clang version | clang-r510928 |
-----