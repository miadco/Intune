# Phase 1.2: Configure Core Endpoint Security Policies

## 🎯 Objective

To harden the Windows 10/11 provisioning process for remote employees using Microsoft Intune by configuring essential security policies including compliance rules, antivirus, BitLocker encryption, and security baselines.

## 🛠️ Tasks I Completed

### ✅ 1. Created a Windows 10/11 Compliance Policy

I enforced BitLocker, secure boot, password requirements, and threat level compliance.

**Screenshot:** `intune-create-compliance-policy-windows10.jpg`
**Caption:** Creating a new compliance policy in Microsoft Intune for Windows 10/11 devices.

**Screenshot:** `intune-compliance-policy-basics-win10.jpg`
**Caption:** Naming the policy "Win10-Compliance-Policy" to apply to all Windows 10 and later devices.

---

### ✅ 2. Configured Microsoft Defender Antivirus Policy

I enabled real-time protection and cloud-delivered protection.

**Screenshot:** `intune-create-defender-antivirus-policy.jpg`
**Caption:** Initiating the creation of a Defender Antivirus policy from the Intune security center.

**Screenshot:** `intune-defender-base-policy-edit.jpg`
**Caption:** Naming the policy "Defender-Base-Policy" for clear identification.

---

### ✅ 3. Created and Configured BitLocker Encryption Policy

I enforced OS drive encryption, backed up recovery keys to AAD, and denied write access to unencrypted drives.

**Screenshot:** `intune-create-bitlocker-policy-windows.jpg`
**Caption:** Creating a BitLocker disk encryption policy within the Intune admin center.

**Screenshot:** `bitlocker-config-part1.jpg`
**Caption:** Configuring BitLocker settings including recovery password rotation for AAD-joined devices.

**Screenshot:** `bitlocker-config-part2.jpg`
**Caption:** Enabling OS drive encryption and specifying "Used Space Only" as the method.

**Screenshot:** `bitlocker-config-part3.jpg`
**Caption:** Leaving most pre-boot and authentication options not configured for automation compatibility.

**Screenshot:** `bitlocker-config-part4.jpg`
**Caption:** Reviewing write access controls for unprotected fixed and removable drives.

---

### ✅ 4. Applied Microsoft Security Baseline

I applied Microsoft-recommended security settings including Defender, Firewall, BitLocker, and SmartScreen.

**Screenshot:** `intune-security-baseline-review-create.jpg`
**Caption:** Reviewing and deploying the Microsoft Defender for Endpoint Security Baseline profile.

---

## 📌 Summary

This phase demonstrates my ability to implement enterprise-grade security controls using Intune. I configured multiple policy layers to ensure a secure and compliant device posture from the first boot—meeting real-world zero-touch onboarding requirements for remote developers.

---

**Next:** Proceed to Phase 1.3 – Application Deployment
