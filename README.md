# BilepterOS: Project Zenshard
https://sites.google.com/view/bilepterosvzenshard/home

---

## Zenshard `.iso` Guide

### 1. Unified Intel & AMD Platforms (Live ISOs)

| CPU Family | Target Processor | Base Tool | Target Architecture Format | Target Build Configuration Output File |
| :--- | :--- | :--- | :--- | :--- |
| **Intel & AMD (64-bit)** | Core / Ryzen / Xeon / EPYC / Athlon 64 | Cubic (Debian) | `x64` | `zenshard-release-x64-generic.iso` |
| **Intel & AMD (32-bit)** | Pentium (TSC) / AMD K6-2 & K6-3 | Cubic (Debian 32) | `x32` | `zenshard-release-x32-legacy.iso` |

### 2. Broadcom / Raspberry Pi Platforms (Flashable Storage Images)

| CPU Family | Target Processor | Base Tool | Target Architecture Format | Target Build Configuration Output File |
| :--- | :--- | :--- | :--- | :--- |
| **Broadcom** | Raspberry Pi Zero W (BCM2835) | Buildroot / rpi-bld | `armv6el` | `zenshard-release-armv6el-pizerow.img` |
| **Broadcom** | Raspberry Pi Zero 2W / Pi 3 (BCM2837) | Buildroot / rpi-bld | `aarch64` | `zenshard-release-aarch64-pi3ubl.img` |
| **Broadcom** | Raspberry Pi 4 (BCM2711) | Buildroot / rpi-bld | `aarch64` | `zenshard-release-aarch64-pi4.img` |
| **Broadcom** | Raspberry Pi 5 (BCM2712) | Buildroot / rpi-bld | `aarch64` | `zenshard-release-aarch64-pi5.img` |

### 3. Allwinner & Olimex Platforms (Flashable Storage Images)

| CPU Family | Target Processor / Board | Base Tool | Target Architecture Format | Target Build Configuration Output File |
| :--- | :--- | :--- | :--- | :--- |
| **Allwinner** | V-Series (V100 IP Camera SoC) | Armbian Framework | `armv7hf` | `zenshard-release-armv7hf-allwinnerv100.img` |
| **Allwinner** | A-Series / H-Series Mainstream (e.g., H616) | Armbian Framework | `aarch64` | `zenshard-release-aarch64-allwinnergen8.img` |
| **Allwinner** | D-Series (D1 Single-Core SoC) | Armbian / Buildroot | `riscv64` | `zenshard-release-riscv64-allwinnerd1.img` |
| **Olimex** | OLinuXino Boards (Allwinner A20 Dual-Core) | Armbian Framework | `armv7hf` | `zenshard-release-armv7hf-olinuxinoa20.img` |

---

## Future Targets

##### 4. NXP i.MX Series
##### 5. Texas Instruments Sitara Series
##### 6. STMicroelectronics Series

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
