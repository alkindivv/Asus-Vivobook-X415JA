# Hackintosh-Asus-Vivoobook-X415JA

[![AsusVivobook](https://img.shields.io/badge/ThinkPad-X230-blue.svg)](https://www.jakartanotebook.com/asus-vivobook-x415ja-a416-bv311ts-intel-core-i3-1005g1-4gb-1tb-14-inch-windows-10-silver)
[![MacOS High Siera](https://img.shields.io/badge/HighSiera-10.15-red.svg)](https://www.apple.com/)
[![MacOS Mojave](https://img.shields.io/badge/Mojave-10.14-red.svg)](https://www.apple.com/)
[![MacOS Catalina](https://img.shields.io/badge/Catalina-10.15-red.svg)](https://www.apple.com/)
[![MacOS BigSur](https://img.shields.io/badge/Big_Sur-11.5-red.svg)](https://www.apple.com/)
[![OpenCore](https://img.shields.io/badge/OpenCore-0.7.1-blue.svg)](https://github.com/acidanthera/OpenCorePkg/releases/latest)

This is my complete EFI folder to be used for hackintosh on Asus Vivobook X415JA notebook with multibooting:
- macOS High Sierra 10.13.x
- macOS Mojave 10.14.x
- macOS Catalina 10.15.x
- macOS Big Sur 11.x
- macOS Monterey 12.x
 
![Screenshot 2021-07-29 at 09 18 24](https://user-images.githubusercontent.com/66145311/128116412-90997bb5-9cc1-40c1-94e2-d65855486eb9.png) 
 
> ## How to Get
- Clone whole repo: $ 'https://github.com/alkindivv/Asus-Vivobook-X415JA.git'
- Download [Specific Folder](https://minhaskamal.github.io/DownGit/#/home?url=https://github.com/alkindivv/Asus-Vivobook-X415JA.git) only.
 
> ## Notebook Specs

- [x] <b>Model</b>: Asus Vivobook X415JA
- [x] <b>CPU</b>: Intel i7-1065G7 (10rd Gen)
- [x] <b>Chipset</b>: Intel® QM77 Express Chipset
- [x] <b>iGPU</b>: Intel UHD Graphics G1 @ 1GB
- [x] <b>RAM</b>: 8GB DDR4 PC25600 / 3200Mhz
- [x] <b>Storage</b>: 512GB Intel NVME (GUID Partition Table)
- [x] <b>Audio</b>: Realtek ALC256 HD Audio Controller
- [x] <b>Wifi</b>: Realtek 8821CE Wirelees LAN 
- [x] <b>Trackpad</b>: ASUE1409 I2C Interface
- [x] <b> Monitor</b>: FHD (1980x1080) 60Mhz
- [x] <b>BOOT Loader</b>: OpenCore r0.7.2
- [x] <b>BOOT Mode</b>: UEFI
- [x] <b>BIOS Version</b>: 5.14
 
> ## EFI Contains
- [x] <b>OpenCore binary, config.plist</b>, drivers for uefi, themes, etc..
- [x] <b>Patched ACPI Tables (DSDT-SSDT)</b> for Sleep, Restart, Shutdown, Touchpad, Brightness, CPU Power Magement etc..
- [x] <b>3rd party kexts</b> for working devices under macOS High Sierra (10.13), macOS Mojave (10.14), macOS Catalina (10.15), macOS BigSur (11) and macOS Monterey BETA (12)
 
<details>
<summary><strong> What's Worked </strong></summary>
<br>

| Feature                              | Status | Dependency          |
| :----------------------------------- | ------ | ------------------- |
| QE/CI Enabled Graphics               | ✅   | Config Inject + WhateverGreen.kext |
| Brightness Adjustments               | ✅   | PNLF SSDT Patch + WhateverGreen.kext |
| CPU Power Management               | ✅   | SSDT Patch |
| Realtek ALC256 Audio out             | ✅   | HDEF SSDT Patch + AppleALC.kext |
| Trackpad ASUE1409 and Track Point     | ✅   | VoodoI2C.kext |
| FN Keys                 | ✅   | SSDT Patch |
| Battery Indicator                    | ✅   | ECEnabler.kext |
| WebCam                               | ✅   | Native |
| USB2.0 Port + USB 3.0 Port           | ✅   | SSDT Patch |
| Sleep and Wake                       | ✅   | SSDT Patch |
| Mac App Store Access                 | ✅   | Native |
| iMessage and FaceTime                | ✅   | if you are using MLB and ROM from original Macs |

</details>

<details>
<summary><strong> List of Gestures </strong></summary>
<br>

| Feature                              | Status | Dependency          |
| :----------------------------------- | ------ | ------------------- |
| 2 Finger Swipe Left and Right                 | ✅   | Forward and Backward. |
| 3 Finger Swipe Left and Right                  | ✅   | Right/Left Space/Full Screen apps switch. |
| 3 Finger Swipe Up And Down                    | ✅   | Toggle Full screen Switch. |
| 4 Finger Swipe Up And Down                   | ✅   | Gestures. |


</details>
 
<details>
<summary><strong> Not Working </strong></summary>
<br>

| Feature                              | Status | Dependency          |
| :----------------------------------- | ------ | ------------------- |
| Builtin WiFI Realtek 8821CE Wirelees LAN                 | ❌   | Unsupported |
| HDMI out and Audio                | ❌   | Common Problem with IceLake Chipset |


</details>
 
<details>
<summary><strong> Not Tested </strong></summary>
<br>

| Feature                              | Status | Dependency          |
| :----------------------------------- | ------ | ------------------- |
| Realtek USB Card Reader                | ❌   | I don't have one of Card Reader. |



</details>
 
> ## Notes

1. macOS versions used are <b>Retail from Mac App Store</b>, using <b>createinstallmedia</b> for USB Installer


<details>
<summary><strong> Credits </strong></summary>
<br>

- [Apple](https://www.apple.com) for macOS.
- [Acidanthera](https://github.com/acidanthera) for all the kexts/utilities that they made.
- [Rehabman](https://github.com/RehabMan) and [Daliansky](https://github.com/daliansky) for the patches and guides and kexts.
- [Dortania](https://github.com/dortania) for for the OpenCore Install Guide.

</details>
