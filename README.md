# Build Recovery using Github Actions

## Release Notes
```
= 2024/11/10 - V1.2
- Corrected the Clang URL and performed cleanups
= 2024/01/14 - V1.1
- Introduced a step to display user inputs
- Organized user inputs for better readability
- Included the codename in the name of the flashable zip
= 2024/01/12 - V1
- Initial version submission
```
-----

## Parameter Description
| Name | Description | Example |
| ------------ | -------------------- | ------------ |
| `Custom Build Title` | Customizes the build title for Telegram notifications | Platina 4.19 KSU |
| `Send Notification` | Determines if a Telegram notification should be sent | ticked |
| `Kernel Tree` | Specifies the kernel source repository | https://github.com/itisFarzin-Phone/kernel_xiaomi_sdm660 |
| `Kernel Tree Branch` | Defines the kernel branch to use | SW-3.2.7-KSU |
| `Phone Codename` | Utilized for building the kernel (**CODENAME**_defconfig) and in notifications | platina |
| `AnyKernel Url` | Provides the AnyKernel repository URL | https://github.com/itisFarzin-Phone/AnyKernel3 |
| `AnyKernel Branch` | Specifies the AnyKernel branch to use | platina |
| `Clang Version` | Selects the Clang version for the build | clang-r510928 |
-----