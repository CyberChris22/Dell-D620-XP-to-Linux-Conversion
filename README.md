<<<<<<< HEAD
# Dell Latitude D620 – Windows XP to Linux Conversion

## Overview

Windows XP is no longer supported by Microsoft, making it unsafe to use on the modern internet due to unpatched vulnerabilities and lack of security updates. This project documents the process of converting a legacy **Dell Latitude D620** laptop from Windows XP to a modern, lightweight Linux distribution suitable for safe, light-duty personal use.

Because upgrading this system to a modern version of Windows would be impractical due to hardware limitations and licensing costs, Linux was selected as the most viable alternative. The goal was to choose a Linux distribution that could operate reliably on legacy hardware while still providing a graphical user interface and basic usability.

---

## Original Operating System

The system originally booted into Windows XP.

![Windows XP boot screen](screenshots/00-XPboot.jpg)

---

## Hardware Specifications

The Dell Latitude D620 hardware specifications are as follows:

- **CPU:** Intel Core 2 Duo T5600 @ 1.83 GHz  
- **Memory:** 1024 MB RAM  
- **Storage:** 80 GB HDD  
- **Optical Drive:** CD-RW / DVD  

![Windows XP system properties](screenshots/01-winxp_system.jpg)

These specifications significantly restrict which modern operating systems can be installed and used reliably.

---

## Linux Distribution Selection

After evaluating several lightweight Linux distributions, the following options were considered:

- **Xubuntu** – Rejected due to higher memory requirements (2 GB RAM recommended)
- **Linux Mint Xfce** – Considered borderline usable on 1 GB RAM
- **Lubuntu** – Selected due to its minimal memory footprint and lightweight desktop environment

**Lubuntu** was chosen because it is specifically designed for low-resource systems and provides a functional graphical desktop while consuming significantly less memory than other Ubuntu-based distributions.

---

## Data Backup

Before modifying the system, important files stored on the Windows XP installation were backed up to external media.

![Transferring files to USB](screenshots/02-winxp_filetransfer.jpg)

![Files safely backed up to USB](screenshots/03-winxp_usbbackup.jpg)

This ensured that no personal data would be lost during the operating system replacement.

---

## Installation Media Preparation

To begin the installation process, the Lubuntu installation media was prepared.

![Lubuntu download page](screenshots/04-Lubuntu_download_page.jpg)

Initially, the plan was to burn the Lubuntu ISO to disc. However, only CD-RW media was available, which is insufficient for modern Linux ISOs. As an alternative, a bootable USB drive was created using Rufus.

![Rufus download page](screenshots/05-Rufus_dl_page.jpg)

![Creating bootable USB with Rufus](screenshots/06-Rufus_create_bootable_usb.jpg)

![Lubuntu ISO on USB](screenshots/07-Lubuntu_ISO_USB.jpg)

![Attempting to boot Lubuntu 24.04 from USB](screenshots/08-booting_24.04_from_USB.jpg)

---

## Boot Media Challenges and Initial Installation Attempt

Due to limitations of the Dell Latitude D620 BIOS, USB booting proved unreliable and resulted in inconsistent behavior. To ensure reliable booting on this legacy system, installation media was recreated using a DVD.

![Burning Lubuntu ISO to DVD](screenshots/09-Burning_ISO_to_DVD.jpg)

The Lubuntu 24.04 LTS installer was launched from DVD:

![Lubuntu installation step](screenshots/10-install-Lubuntu1.jpg)
![Lubuntu installation step](screenshots/11-install-Lubuntu2.jpg)
![Lubuntu installation step](screenshots/12-install-Lubuntu3.jpg)
![Lubuntu installation step](screenshots/13-install-Lubuntu4.jpg)

![Lubuntu login screen](screenshots/14-Lubuntu_login.jpg)

---

## Lubuntu 24.04 LTS Compatibility Issues

Although Lubuntu 24.04 LTS installed successfully, the system experienced persistent graphical login loops after installation. Despite troubleshooting efforts, the desktop environment failed to load reliably.

This behavior was determined to be caused by the combination of:
- Only **1 GB of RAM**
- Legacy Intel graphics hardware
- Increased resource requirements of newer desktop components in 24.04 LTS

As a result, Lubuntu **22.04 LTS** was selected as a more suitable alternative due to its lighter memory footprint and better compatibility with legacy hardware.

![Burning Lubuntu 22.04 ISO](screenshots/15-Lubuntu_22.04_burn.jpg)

---

## Lubuntu 22.04 LTS Installation

The Lubuntu 22.04 LTS installer booted successfully from DVD.

![Booting Lubuntu 22.04 from DVD](screenshots/16-22.04_boot_from_DVD.jpg)

![Try or Install Lubuntu menu](screenshots/17-try-or-install-Lubuntu-22.04.jpg)

![Lubuntu home screen before installation](screenshots/18-Lubuntu_home_screen_before_22.04_install.jpg)

![Lubuntu 22.04 install icon](screenshots/19-Lubuntu_22.04_install_icon.jpg)

![Lubuntu 22.04 installer](screenshots/20-Lubuntu_22.04_installer.jpg)

![Replacing Lubuntu 24.04 with 22.04](screenshots/21-Installing_22.04_removing_24.04.jpg)

![Lubuntu 22.04 installation complete](screenshots/22-Lubuntu_installation_complete.jpg)

---

## Post-Installation Updates

After installation, the system was updated to ensure it received the latest security patches.

![Post-installation system updates](screenshots/23-Post_installation_updates.jpg)

A total of **226 security updates** were applied.

---

## Conclusion

This project demonstrates the successful conversion of a legacy Dell Latitude D620 laptop from Windows XP to a secure and usable Linux system. Through careful evaluation of hardware limitations, multiple installation attempts, and troubleshooting boot and compatibility issues, Lubuntu 22.04 LTS was identified as the optimal solution.

The final system provides:
- A supported operating system
- A functional graphical desktop
- Improved security for internet use
- Extended usability of legacy hardware

This conversion highlights the value of lightweight Linux distributions in extending the life of older systems while maintaining safety and usability.
=======
# Dell-D620-XP-to-Linux-Conversion
Converting a Dell Latitude D620 laptop from Windows XP to a lightweight Lubuntu Linux system.
>>>>>>> 3f66231395695d9ba135717b173e18a94cf93239
