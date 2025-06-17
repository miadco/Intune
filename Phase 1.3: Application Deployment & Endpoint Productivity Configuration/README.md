## Phase 1.3: Application Deployment & Productivity Configuration

**Objective:**
My goal in this phase was to automate the deployment of essential productivity and security applications using Microsoft Intune. I wanted to demonstrate my ability to configure and assign critical software and system policies, laying the foundation for a seamless and productive user experience from the moment of enrollment.

---

### ✅ Tasks Completed

#### 1. Microsoft 365 Apps Deployment

I configured the deployment of the Microsoft 365 Apps suite to ensure all users have access to core productivity tools.

* **Action:** I created a new Windows app deployment for Microsoft 365 Apps.
* **Configuration:** I selected the Current update channel and included core applications: Word, Excel, Outlook, and Teams.
* **Assignment:** I targeted the deployment to a device group, simulating a standard production rollout.

**Screenshot:**
![Configuring the Microsoft 365 Apps suite](intune-add-m365-apps-select-type.jpg)

**Screenshot:**
![Assigning M365 Apps deployment](intune-m365-apps-review-create.jpg)

---

#### 2. Microsoft Edge Browser Deployment

I ensured a modern, secure browser is installed and managed on all endpoints.

* **Action:** I added Microsoft Edge (Stable Channel) from the built-in Intune app catalog.
* **Configuration:** I set the installation to use the operating system's default language for a seamless user experience.
* **Context:** I deployed it in the System context to ensure successful installation without requiring user interaction.

**Screenshot:**
![Selecting Microsoft Edge Stable channel](intune-add-edge-app-info.jpg)

**Screenshot:**
![Finalizing Edge deployment assignment](intune-add-edge-app-settings.jpg)

---

#### 3. OneDrive Known Folder Move (KFM) Policy

I proactively configured a policy to back up critical user data to the cloud, protecting against data loss and enabling cross-device synchronization.

* **Action:** I created a configuration profile using the Settings Catalog, Intune's modern policy management interface.
* **Policy:** I enabled "Silently move Windows known folders to OneDrive," which automatically redirects the user's Desktop, Documents, and Pictures folders to their OneDrive account.
* **Readiness:** The policy is fully configured and ready for deployment; it only requires a valid Tenant ID to function in a live environment.

**Screenshot:**
![Configuring OneDrive KFM policy in catalog](intune-kfm-onedrive-profile-create.jpg)

**Screenshot:**
![Enabling OneDrive KFM setting](intune-settings-catalog-onedrive-kfm.jpg)

---

### 📌 Implementation Summary

This phase demonstrates my proficiency in managing the complete application and productivity lifecycle within Microsoft Intune. From an administrator's perspective, all configurations are complete and staged for deployment. I've successfully built the logic to deploy essential software (Microsoft 365, Edge) and enforce critical data protection policies (OneDrive KFM) without requiring manual intervention on the endpoint.

This setup is foundational for zero-touch provisioning. When a device is eventually enrolled, it will be automatically equipped with the necessary tools and safeguards for immediate productivity.

---

### 🚀 Optional: Phase 1.4 – Device Enrollment & Validation

The logical next step is to validate the end-to-end deployment lifecycle on a test device. This involves enrolling a Windows 11 VM into the tenant, allowing it to sync with Intune, and verifying that all configured applications and policies are successfully applied. This optional final step would complete the full Create > Assign > Enforce > Validate workflow.
