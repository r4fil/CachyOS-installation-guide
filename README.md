# 🚀 CachyOS Installation & Setup Guide

CachyOS installation for beginners — a simple, step-by-step guide to download, install, and optimize CachyOS for maximum speed and gaming performance.

---

### 📌 What is CachyOS, and why use it?
<details>
<summary><b>▶ Click here for info</b></summary>

<br>

* **Beginner-Friendly Arch Linux:** Gives you all the speed and latest software of Arch Linux without complex manual setup.
* **Extreme Speed:** Uses custom-built kernels optimized for your CPU to make apps and games run noticeably smoother.
* **Pre-Configured for Gaming:** Comes out of the box with built-in support for Steam, custom Proton builds, and performance tools.

</details>

---

### 📥 1. How to Download the ISO
<details>
<summary><b>▶ Click here for info</b></summary>

<br>

1. Visit the official CachyOS download page: [cachyos.org/download](https://cachyos.org/download).
2. Choose **Desktop Edition (x86_64)**.
3. Click **Direct Download** to get the `.iso` file.

</details>

---

### 🔌 2. Making a Bootable USB Drive
<details>
<summary><b>▶ Click here for info</b></summary>

<br>

1. Download **Rufus** (`rufus.ie`) or **BalenaEtcher**.
2. Insert a USB flash drive (**8 GB or larger**).
3. Select your downloaded CachyOS `.iso` file.
4. If using Rufus, choose **DD Image mode** when prompted, then click **START**.

</details>

---

### ⚙️ 3. BIOS / UEFI Settings (Before Installing)
<details>
<summary><b>▶ Click here for info</b></summary>

<br>

Restart your PC and tap `DEL` or `F2` to enter your BIOS, then change these settings:

* **Secure Boot:** Disabled ❌
* **Fast Boot:** Disabled ❌
* **SATA / Storage Mode:** AHCI 
* **Boot Mode:** UEFI

</details>

---

### 🛠️ 4. Step-by-Step Installation
<details>
<summary><b>▶ Click here for info</b></summary>

<br>

1. Boot your PC from the USB drive.
2. Select **Launch Installer** (Choose **Online Installer**).
3. **Desktop Choice:** Pick **KDE Plasma** (recommended for beginners and gamers).
4. **Graphics Driver:**
   * Select **NVIDIA (Proprietary)** if you have an NVIDIA GPU.
   * Select **Open-Source / AMD / Intel** if you have AMD or Intel graphics.
5. **Partitioning:** Select **Erase Disk** for automatic setup, and choose **BTRFS** as the filesystem.
6. Set your username and password, then click **Install**.

</details>

---

### ⚡ 5. First Commands to Run After Installation
<details>
<summary><b>▶ Click here for info</b></summary>

<br>

Open the terminal after booting into CachyOS and run these commands to update and install gaming software:

```bash
# Update mirror speed and system packages
sudo cachyos-rate-mirrors
sudo pacman -Syu

# Install gaming software (Steam, Wine, Lutris)
sudo pacman -S steam lutris wine-staging proton-cachyos

