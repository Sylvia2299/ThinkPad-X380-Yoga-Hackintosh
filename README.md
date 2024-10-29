# Lenovo ThinkPad X380 Yoga - OpenCore Configuration

<img align="right" src="https://p1-ofp.static.pub/medias/bWFzdGVyfHJvb3R8MzY5NzQ4fGltYWdlL3BuZ3xoMTEvaGMwLzE0NDQ4MTg0NTI0ODMwLnBuZ3wyZjE4MmQ5YmEyN2U1M2VhOTJkZDM4NzFjMTUzNDk2M2NmOGQ5OTQ2MjYxNTVlNjY3YmYxMTU4ZDM2Y2RmNjlk/lenovo-laptop-thinkpad-x380-2-in-1-hero.png" alt="macOS running on the X380 Yoga" width="425">

[![macOS](https://img.shields.io/badge/macOS-Sonoma-brightgreen.svg?logo=apple)](https://developer.apple.com/documentation/macos-release-notes)
[![macOS](https://img.shields.io/badge/macOS-Sequoia-brightgreen.svg?logo=apple)](https://developer.apple.com/documentation/macos-release-notes)
[![OpenCore](https://img.shields.io/badge/OpenCore-1.0.2-blue.svg)](https://github.com/acidanthera/OpenCorePkg)
[![Model](https://img.shields.io/badge/Model-20KLH-9cf)](https://psref.lenovo.com/syspool/Sys/PDF/ThinkPad/ThinkPad_X380_Yoga/ThinkPad_X380_Yoga_Spec.PDF)
[![BIOS](https://img.shields.io/badge/BIOS-1.41-blue)](https://pcsupport.lenovo.com/us/en/products/laptops-and-netbooks/thinkpad-x-series-laptops/thinkpad-x380-yoga/downloads/driver-list/component?name=BIOS%2FUEFI&id=5AC6A815-321D-440E-8833-B07A93E0428C)
[![License](https://img.shields.io/badge/license-MIT-purple.svg)](/LICENSE)
[![issues](https://img.shields.io/github/issues/kotakbiasa/ThinkPad-X380-Yoga-Hackintosh-OpenCore)](https://github.com/kotakbiasa/ThinkPad-X380-Yoga-Hackintosh-OpenCore/issues)
[![last commit](https://img.shields.io/github/last-commit/kotakbiasa/ThinkPad-X380-Yoga-Hackintosh-OpenCore)](https://github.com/kotakbiasa/ThinkPad-X380-Yoga-Hackintosh-OpenCore)

**DISCLAIMER:**  
This OpenCore EFI works fine on my Thinkpad X380 Yoga.
I am not responsible for any damages you may cause.  
As you embark on your Hackintosh journey you are encouraged to **READ** the entire README and [Dortania](https://dortania.github.io/getting-started/) guides before you start to get an understanding of the install process. It will save many a message instructing you to read the manual. **I am not an expert**, I haven't forced you to do anything, so put on your big boy pants and take responsibility for any mess you get yourself into.

With that said I'm happy to help when/where I can. When you encounter bug or want to improve this repo, consider opening an issue or pull request. You can also find a wealth of knowledge on [Reddit](https://www.reddit.com/r/hackintosh/), [TonyMacX86](https://www.tonymacx86.com) or [Google](https://www.google.com).

## 💻 My Hardware

| Category  | Component                                            | Note                                                         |
| --------- | ---------------------------------------------------- | ------------------------------------------------------------ |
| Type      | 20LH                                                 |                                                              |
| CPU       | Intel(R) Core(TM) i5-8350U CPU @ 1.70GHz             |                                                              |
| GPU       | Intel UHD 620                                        |                                                              |
| SSD       | Lexar NM620 512GB M.2 NVMe SSD                       | Replaced cursed PM 981 which still doesn't work reliably. Read this [Anti-Hackintosh Buyers Guide - Storage](https://dortania.github.io/Anti-Hackintosh-Buyers-Guide/Storage.html)     |
| Screen    | 13.3" FHD 1920x1080                                  | Multi touch and pen* support working                         |
| Memory    | 16GB DDR4 2400Mhz                                    |                                                              |
| Camera    | 720p Camera + IR Camera                              |                                                              |
| Audio     | Conexant® CX8200                                     | I suggest trying several layout ID `3, 15, 21, 23, or 80`    |
| Touchoad  | ELAN v4 LEN2034 PS2 Interace                         |                                                              |
| Wifi & BT | Intel AC 8265 and Bluetooth                          | Use AirportItlwm for your macOS version and enjoy native Wi-Fi control. |
| Ethernet  | Intel I219-LM4 Gigabit Ethernet                      |                                                              | 
| Input     | PS2 Keyboard & I2CHID TrackPad (touchscreen and pen) | I'm using [YogaSMC](https://github.com/zhen-zen/YogaSMC) for media keys. The kext is in the folder but **you'll need to install the app.** |

<p align="center">
  <img src="/img/x380-yoga_seqoia.png">
</p>