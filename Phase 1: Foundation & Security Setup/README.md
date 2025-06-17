✅ Phase 1: Foundation & Security Setup
Time Estimate: 60–90 minutes
Objective: Prepare the Intune environment and establish core security + compliance infrastructure.

🧷 Tasks
🧪 Create a Microsoft 365 Developer Tenant

https://developer.microsoft.com/en-us/microsoft-365/dev-program

Choose the E5 license for full Intune/Endpoint Manager access.

🧑‍💼 Enroll Windows 11 Device into Intune

Use a Windows 11 Pro VM or physical machine.

Log in with a test user (e.g., jdoe@yourtenant.onmicrosoft.com) and confirm automatic MDM enrollment via Azure AD Join.

🔐 Create Compliance Policy

Require BitLocker encryption.

Require secure password (min length, complexity).

Block jailbroken/rooted devices (if applicable).

🛡️ Create Device Configuration Profile

Enforce security baselines: Windows Defender Antivirus, firewall, OneDrive redirection, etc.

Deploy custom settings like company branding or Start menu layout (optional polish).

🧙‍♂️ Create a Dynamic Azure AD Group for Autopilot or Intune-targeted devices

Example rule:

plaintext
Copy
Edit
(device.deviceOSType -eq "Windows") and (device.deviceOwnership -eq "Company")
Assign all compliance/configuration policies to this group.

📸 Screenshots to Capture:

Microsoft 365 tenant dashboard

Endpoint Manager homepage

Compliance policy setup

Configuration profile summary

Dynamic group creation and rule
