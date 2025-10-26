# 🪟 TPE — Customized Windows PE (x64)

**TPE** is a customized Windows Preinstallation Environment (WinPE) distribution (x64) based on WEPE & Windows PE.  
It bundles a graphical set of maintenance, recovery, and deployment utilities and includes additional driver and hardware support for modern systems.

> ⚠️ **Educational use only.** This project is intended for testing, learning, and legitimate maintenance/administration tasks only. Do not use it for illegal or unauthorized access. Misuse may be unlawful.

---

## 📦 Download

Prebuilt x64 image and additional files:

🔗 **Mega.nz:** https://mega.nz/folder/2A9QXTwR#thFzHUEYrMwsybk1rN4-QQ

> The upload includes:
> - A prebuilt x64 TPE image
> - Files to copy to a USB drive

---

## 💿 Create a Bootable USB (FAT32, < 32 GB)

**Important:** The USB drive must be FAT32 and **less than 32 GB**. This process will overwrite the drive — back up any important data.

1. Format your USB drive as **FAT32** and ensure it is empty.
2. Download and extract the archive from the Mega link above.
3. From the extracted folder, locate the `1v0.1.2` directory.
4. **Copy everything under the `1v0.1.2` folder** directly to the **root** of the USB drive.

Example final layout:
USB_DRIVE:
├── boot
├── sources
├── EFI
├── bootmgr
└── bootmgr.efi

5. Insert the USB into the target machine and boot from it using the system boot menu (BIOS/UEFI).

---

## 🔧 High-level Feature Overview

TPE aims to provide a GUI-first environment for lawful system maintenance, diagnostics, and deployment. High-level capabilities include:

- Modern hardware support (touchpads, high-DPI screens, SD Drives, Intel RST/RAID metadata handling, common NVMe controllers, etc.)
- Tools and GUI workflows to assist with migrating older Windows installations to modern hardware (boot repair workflows, driver injection helpers, guidance for preparing systems)
- GUI-driven utilities for image deployment, unattended setup helpers, and group deployment workflows for IT environments
- Graphical tools for data recovery, partition inspection, file restoration, and system cleanup/trimming
- Utilities to customize and slim Windows images (image management helpers; non-destructive tools for administrators)
- GUI wrappers around commonly used forensic and recovery utilities to simplify authorized maintenance tasks

> ⚠️ NOTE: Any features that touch accounts, passwords, or encrypted volumes are provided **only** as tools for authorized recovery or diagnostics and **do not** include or endorse ways to bypass security protections. For encrypted volumes (BitLocker, etc.), users must follow official recovery channels (recovery keys, organizational IT procedures, or Microsoft account recovery) unless they have explicit legal authorization and evidence of ownership.

---

## ⚖️ Legal, Ethical & Security Notice (Read Carefully)

- This repository and its prebuilt images are provided **for educational, testing, and legitimate maintenance/administration use only**. Do **not** use the software to access devices or data without explicit authorization from the device owner.
- I will not assist with or provide instructions for bypassing password protections, evading account protections, or decrypting BitLocker/other full-disk encryption for devices you do not own or have explicit authorization to service.
- Redistribution of Microsoft system files or other third-party binaries may be restricted by license. This repo contains build scripts and documentation so users can rebuild images using official Microsoft ADK/WinPE components.
- Users are responsible for complying with local laws, organizational policies, and software licensing terms when using TPE or the provided images.

Responsible, lawful use helps vendors (including Microsoft) improve security by enabling researchers and administrators to test, report, and fix vulnerabilities.

---

## 🧭 How to Use (GUI-first)

- Boot into TPE from USB.
- Use the Start menu (press the **Windows key** inside the environment) to access included apps and utilities.
- You may find interesting tools under WEPE/Program Files/...
- Most common tasks are exposed through graphical menus—no command-line required for typical recovery and maintenance workflows.

---

## 🛠️ Repository Contents

This repository is intended to contain:
- Build scripts and configuration (PowerShell / batch files, DISM steps, unattend templates) — **no redistributed Microsoft system files included**.
- Documentation for customizing, rebuilding, and adding drivers.
- README (this file), LICENSE, and contribution guidelines.

If you use this repo as a base, obtain required ADK/WinPE components from Microsoft and follow their licensing terms.

---

## 🔐 Account / Encryption Tools — Authorized Use Only

This project may include GUI tooling that *assists administrators* with legitimate account recovery workflows and with diagnosing encrypted volumes **when legal authorization is present**. It **does not** provide or endorse methods for unauthorized access or decryption. If you are not the owner or an authorized administrator for a device, stop and follow official recovery/legal channels.

---

## 📝 License

Scripts and documentation in this repository are released under the **MIT License**.  
Prebuilt binaries are provided via the external Mega link — users are responsible for ensuring they comply with Microsoft licensing and applicable laws.

---

## 👥 Responsible Disclosure & Contributions

- If you find a security vulnerability, follow a responsible disclosure process. Do not use vulnerabilities to access devices without authorization.
- Contributions are welcome for drivers, documentation, and build improvements. Pull requests should avoid including copyrighted Microsoft binaries.
- If contributors propose content related to account or encryption recovery, maintainers may request proof of authorization before accepting workflows or images that could be sensitive.

---

## 👤 Author / Maintainer

- **Author:** [Timothy Y]  
- **Repository:** [https://github.com/yourusername/your-repo-name](https://github.com/Timothy099qw/WinPE_x64/)  
- **Version:** 0.1.2

---
