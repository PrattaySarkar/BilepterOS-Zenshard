# BilepterOS: Project Zenshard
https://sites.google.com/view/bilepterosvzenshard/home

## `.iso` Guide:

| CPU Architecture / Family | Targets | ISO File |
| :--- | :--- | :--- |
| **Intel & AMD (64-bit)** | Core i3/i5/i7/i9, Core 2 Duo, Ryzen, EPYC, Athlon 64 | `zenshard-release-x64.iso` |
| **Intel & AMD (Legacy 32-bit)** | Pentium (with TSC), early Pentium 4, AMD K6-2 / K6-3 | `zenshard-release-x32.iso` |
| **Broadcom / Raspberry Pi** | Zero W, Zero 2W, Pi 3, Pi 4, Pi 5 (BCM2837, BCM2711, BCM2712) | `zenshard-release-buildrt.iso` |
| **Allwinner** | V-Series (V100), A-Series, H-Series, D-Series (RISC-V) | `zenshard-release-armbm.iso` |
| **Olimex** | OLinuXino Boards (A20, etc.) | `zenshard-release-armbm.iso` |
| **NXP** | i.MX Series (i.MX6, i.MX8, i.MX9) | `zenshard-release-armbm.iso` *or* `zenshard-release-buildrt.iso` |
| **Texas Instruments** | Sitara Series (AM335x / AM6x) | `zenshard-release-buildrt.iso` |
| **STMicroelectronics** | STM32MP1 / STM32MP2 | `zenshard-release-buildrt.iso` |

---

## FAQ:

### What is it?
An Linux-Based Operating system for Various Embedded CPUs And Mordern x86_64 CPUs.

### How do I Use it?

#### Before you begin:

1. A USB Flash Drive: Minimum 8GB recommended. (Note: This process will erase all data on the drive).
2. Rufus: Download the latest version from the [official Rufus website](https://rufus.ie).
3. ISO File: Refer to `.iso` **Guide** and download `.iso` From `Releases` Accordingly.

#### Steps to Flash:

1. Next to Boot selection, leave it as Disk or ISO image.
2. Click the SELECT button on the right.
3. Browse your computer, select your downloaded `.iso` file, and click Open.
4. Partition scheme: Select MBR.
5. Target system: Select BIOS or UEFI (or BIOS or UEFI-CSM).
6. File system: Rufus will usually auto-select` FAT32`. If not, Select `FAT32`.
7. Click the START button at the bottom.
8. A prompt titled ISO Image Hybrid Detection will likely appear.
9. Select Write in ISO Image mode (Recommended) first and click OK

#### Steps to Boot:

1. Shut down the computer completely.
2. Insert the USB drive.
3. Turn the computer on and immediately start tapping the Boot Menu Key repeatedly until a menu appears. Common Boot Menu keys: F12 (Dell, Lenovo, Gigabyte), F11 (MSI, AsRock), F9 (HP), or Esc (ASUS).
4. Select your USB drive from the list. If you are booting on a UEFI system, choose the option prefixed with `UEFI:`, or else choose the USB.
5. A menu will appear, select `ZenshardOS Live System` if you want to try out the system, or else select `ZenshardOS Graphical Installer` to install ZenshardOS.

## Contribution & License.

This project is licensed under Apache 3.0 License, We are open to Contributions.
