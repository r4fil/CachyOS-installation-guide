# CachyOS: Beginner’s Installation & Setup Guide

A simple, straightforward guide to downloading, flashing, and installing **CachyOS**—an Arch Linux-based distribution optimized for speed, low latency, and modern gaming.

---

## 🚀 Why Choose CachyOS?

CachyOS is designed to make Arch Linux fast and easy to use without the complicated manual setup.

* **Optimized Performance:** Uses custom x86-64 CPU-optimized packages (v3/v4) for faster app launches and smoother system responsiveness.
* **Gaming Ready:** Includes out-of-the-box support for Nvidia/AMD graphics drivers, Steam, Lutris, Proton, and custom kernel tweaks for gaming performance.
* **Beginner Friendly Installer:** Uses the Calamares graphical installer so you can set up your system visually without typing terminal commands.

---

## 1. Pre-Installation Checklist

Before starting, make sure you have:
* A USB flash drive (**8GB or larger**).
* An active internet connection (Ethernet or Wi-Fi).
* Backed up any important files on your PC and USB drive.

---

## 2. Downloading CachyOS

Always get the official ISO file directly from the source:

* **Official Website:** [cachyos.org](https://cachyos.org)
* **SourceForge / Mirrors:** Select the **Desktop Edition** ISO (x86-64-v3 if supported by your CPU, or the standard x86-64 build).

---

## 3. Creating a Bootable USB Drive

### On Windows (Using Rufus):
1. Plug in your USB drive.
2. Open **Rufus** and select your USB drive under **Device**.
3. Click **Select** and choose the downloaded CachyOS ISO.
4. Set the partition scheme to **GPT** (for modern UEFI systems).
5. Click **Start** (if prompted, choose **DD Image mode**).

### On Linux (Using Ventoy or BalenaEtcher):
* You can simply copy the ISO file onto a **Ventoy** USB drive or write it using **BalenaEtcher**.

---

## 4. Booting and Installing

1. Shut down your PC and plug in the bootable USB drive.
2. Power on your PC and hit your motherboard’s **Boot Menu Key** (usually `F12`, `F11`, `F8`, or `Del`).
3. Select your USB drive from the UEFI boot options.
4. Once the live desktop loads, click **Launch Installer**.
5. Follow the step-by-step setup:
   * **Language & Location:** Set your keyboard layout and timezone.
   * **Desktop Environment:** Select your preferred desktop layout (KDE Plasma is recommended for beginners).
   * **Partitioning:** Choose *Erase Disk* for a clean install, or manually partition if dual-booting alongside Windows.
   * **User Setup:** Enter your username and password.
6. Click **Install** and wait for the process to complete. Reboot when finished and remove the USB drive.

---

## 5. Recommended Post-Install Steps

Once you log in for the first time:

### A. Update the System
Open a terminal and refresh your package database:

```bash
sudo cachyos-bugreport
sudo pacman -Syu
