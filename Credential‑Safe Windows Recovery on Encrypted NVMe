---
title: "Credential‑Safe Windows Recovery on Encrypted NVMe Drive"
date: 2026-01-10
tags:
  - IAM
  - Cloud Security
  - Credential Safety
  - BitLocker
  - Windows Recovery
  - Bootloader (BCD)
  - Data Integrity
  - Incident Response
  - Forensic Documentation
  - OneDrive
  - System Hardening
---

# Credential‑Safe Windows Recovery on Encrypted NVMe Drive  
### A Case Study in IAM, Cloud Security, and System Integrity

## Overview
This project documents a full recovery of a Windows 11 system stored on a BitLocker‑encrypted NVMe drive after a cloning‑related bootloader failure. The goal was not just to restore functionality, but to preserve **credential safety**, **identity integrity**, and **cloud‑synced data** while applying structured, forensic‑style troubleshooting.

This case study demonstrates IAM‑aligned thinking:  
- Protecting identity‑linked encryption keys  
- Maintaining cloud account integrity  
- Ensuring secure boot paths  
- Preserving data governed by identity (OneDrive)  
- Documenting actions for auditability and repeatability  

---

## Objectives
- Restore a non‑booting Windows 11 system without compromising identity‑linked data  
- Maintain BitLocker key integrity and avoid credential exposure  
- Validate cloud‑synced data continuity (OneDrive)  
- Rebuild a clean, trustworthy bootloader  
- Document the process as a repeatable IAM/Cloud Security artifact  

---

## Key Actions

### 1. **BitLocker Decryption & Credential Safety**
- Verified encryption state using `manage-bde -status`
- Fully decrypted the NVMe drive before attempting repairs  
- Ensured recovery key remained protected and logged securely  
- Treated the recovery key as a credential requiring IAM‑level handling  

### 2. **Identity‑Linked Data Preservation (OneDrive)**
- Confirmed all personal files were cloud‑synced  
- Ensured OneDrive account integrity before OS repair  
- Validated that cloud data remains intact even when the local OS is replaced  

### 3. **Bootloader & System Integrity Validation**
- Inspected BCD entries with `bcdedit /enum all`
- Identified misaligned boot paths caused by cloning  
- Rebuilt the bootloader using:  
  `bcdboot C:\Windows /s C: /f UEFI`
- Ensured the system would trust the correct OS partition  

### 4. **Drive Letter & Partition Verification**
- Used `diskpart` to confirm correct volume mapping  
- Identified WinRE drive letter reassignments  
- Disconnected the HDD to prevent cross‑partition contamination  

### 5. **Secure ISO Acquisition & Deployment**
- Downloaded Windows 11 ISO on a mobile device (S22 Ultra)  
- Transferred ISO to Ventoy USB using a USB‑C adapter  
- Ensured ISO integrity and avoided untrusted sources  
- Booted via UEFI‑compliant Ventoy environment  

### 6. **Clean Install with Identity Preservation**
- Performed a clean Windows 11 install on the NVMe OS partition  
- Allowed Windows to auto‑activate using embedded license  
- Reconnected OneDrive to restore cloud‑synced data  

---

## Outcome
- System restored with a clean, trustworthy Windows 11 installation  
- Identity‑linked data preserved through OneDrive  
- Bootloader integrity re‑established  
- BitLocker decryption and credential handling documented  
- Recovery process aligned with IAM and Cloud Security principles  

---

## Skills Demonstrated
- Identity‑linked encryption management (BitLocker)  
- Cloud data continuity (OneDrive)  
- Bootloader integrity and secure boot paths  
- Forensic‑style documentation and incident response  
- Cross‑platform recovery workflows (mobile → USB → UEFI)  
- System hardening and credential safety  

---

## Why This Matters for IAM & Cloud Security
This project shows the ability to:

- Protect identity‑linked assets during system failure  
- Maintain cloud account integrity under stress  
- Understand how encryption, identity, and OS trust interact  
- Document actions in a way that supports auditability  
- Apply structured reasoning to ambiguous system states  

These are core competencies for IAM and Cloud Security roles.
