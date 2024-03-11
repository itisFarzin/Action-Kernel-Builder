# Build Kernel using Github Actions

## Release Notes
```
= 2024/01/29 - V1.3
- fix typos
- change LICENSE
- change description
- make the location of defconfig dynamic
- separate device codename from defconfig name
- add tutorial for how to setup telegram bot
= 2024/01/29 - V1.2
- correcting the path of flashable zip in action artifact
- adding option to upload outputs into a release instead of artifact
- add continue on error for "Send Telegram notification for failure" when it get failed to not getting failed run
= 2024/01/14 - V1.1
- Adding a step to showing user inputs
- User input rearranged
- Codename in the name of the flashable zip
= 2024/01/12 - V1
- The first available version is submitted.
```
-----

## Parameter Description (for platina)
| Name | Description | Example |
| ------------ | -------------------- | ------------ |
| `Custom Build Title` | Set a custom build title when senfing notification to the the Telegram | Platina 4.19 KSU |
| `Send Notification` | Send notification to the Telegram | ticked |
| `Kernel Tree` | Kernel address | https://github.com/itisFarzin/kernel_xiaomi_sdm660 |
| `Kernel Tree Branch` | Kernel branch | SW-3.2.7-KSU |
| `Defconfig location` | Location of defconfig | empty |
| `Defconfig name` | Name of defconfig | platina |
| `Device Codename` | Codename of device | platina |
| `AnyKernel Url` | AnyKernel address | https://github.com/itisFarzin/AnyKernel3 |
| `AnyKernel Branch` | AnyKernel branch | platina |
| `Clang Version` | Clang version | clang-r510928 |
-----

## Parameter Description (for zahedan)
| Name | Description | Example |
| ------------ | -------------------- | ------------ |
| `Custom Build Title` | Set a custom build title when senfing notification to the the Telegram | Platina 4.19 KSU |
| `Send Notification` | Send notification to the Telegram | ticked |
| `Kernel Tree` | Kernel address | https://github.com/itisFarzin/kernel_daria_mt6877 |
| `Kernel Tree Branch` | Kernel branch | zahedan-ksu |
| `Defconfig location` | Location of defconfig | vendor |
| `Defconfig name` | Name of defconfig | k6877v1_64_k419 |
| `Device Codename` | Codename of device | zahedan |
| `AnyKernel Url` | AnyKernel address | https://github.com/itisFarzin/AnyKernel3 |
| `AnyKernel Branch` | AnyKernel branch | zahedan |
-----

## (Optional) Sending Notification and Release
For doing it, you need to set 2 secrets
- **TELEGRAM_CHAT**: the chat id of channel/group you want the notification send to it
- **TELEGRAM_TOKEN**: the token of the bot you created

for adding this secrets, go to the settings of repo then open Secrets and variables and after that click on Actions
via using 'New repository secret' button, you can add secrets to repo