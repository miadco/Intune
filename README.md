# Intune Lab: Zero-Touch Onboarding for a Remote Developer

This project demonstrates an automated endpoint provisioning and security hardening process using Microsoft Intune. The goal was to simulate the onboarding of a new remote developer, ensuring their device is secure, configured for productivity, and equipped with necessary tools from the very first login—with no manual IT intervention required.

### 🔑 Key Skills Demonstrated

* Azure AD Join & Automatic Intune Enrollment
* Security Policy Enforcement (BitLocker, Defender AV)
* Configuration Profiles (Settings Catalog)
* Automated Data Protection (OneDrive Known Folder Move)
* Win32 Application Packaging & Deployment
* PowerShell Scripting for Device Customization

### ⚙️ Workflow & Results

#### 1. Security & Compliance

A compliance policy was created to enforce BitLocker encryption and ensure Microsoft Defender AV is active. This mitigates security risks from device loss or malware.

📸 *(Insert screenshot of compliance policy success in Intune)*

#### 2. Automated Data Protection

A configuration profile was deployed to silently enable OneDrive Known Folder Move. This protects user data by syncing the Desktop, Documents, and Pictures folders to the cloud.

📸 *(Insert screenshot of OneDrive configuration profile success)*

#### 3. App Deployment & Device Customization

Visual Studio Code was deployed as a required Win32 app. A PowerShell script was used to create a "Developer Portal" shortcut on the desktop, linking to internal resources.

📸 *(Insert screenshot of the final desktop with VS Code and the shortcut)*

### 💼 Business Impact

This automated workflow significantly reduces IT workload for new hires, enhances security posture for remote devices, and accelerates time-to-productivity. It provides a consistent, secure, and scalable onboarding experience.

---

## 🧠 Final Resume Bullet Points

* Engineered a zero-touch Windows provisioning workflow using Intune and Azure AD Join, reducing onboarding time and IT overhead
* Hardened endpoint security by deploying compliance policies to enforce BitLocker and Defender AV
* Automated critical data protection with OneDrive Known Folder Move via Intune configuration profiles
* Packaged and deployed Win32 apps and PowerShell automation scripts for scalable endpoint configuration
