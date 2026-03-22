# BYOD Policy for AEC Firms
**Open IT Policy Library for AEC by Sorted Solution** | [sortedsolution.com](https://www.sortedsolution.com/oitpl)<br>
*Version 1.0 — March 2026*
*Free to use, fork, and adapt at [github.com/sortedsol/Open-IT-Policy-Library](https://github.com/sortedsol/Open-IT-Policy-Library)* | [Download DOCX version](https://github.com/sortedsol/Open-IT-Policy-Library/raw/main/policies/aec/BYOD-Policy-AEC.docx)

---

## 1. Purpose

This policy defines the rules for using personal devices — laptops, tablets, and phones — to access the firm's network, email, files, and applications. "BYOD" stands for Bring Your Own Device.

AEC firms deal with sensitive client data, large project files, and licensed software that makes BYOD more complicated than in other industries. This policy balances the flexibility employees want with the security the firm and its clients require.

---

## 2. Scope

This policy applies to anyone who uses a personally owned device to access the firm's resources — employees, contractors, subconsultants, and interns.

"Firm resources" includes:

- Firm email (Microsoft 365, Google Workspace)
- Cloud storage and collaboration platforms (SharePoint, OneDrive, Dropbox, BIM 360, Autodesk Docs, Bluebeam Studio, BIMcloud)
- The firm's VPN
- Firm-managed applications and project management tools
- Any system you log into with firm credentials

This policy does **not** cover firm-owned devices that employees take home — those are covered by the firm's Acceptable Use Policy.

---

## 3. Who Can Use Personal Devices

BYOD is not automatic. You need IT approval before using a personal device for firm work.

!!! tip "Firm administrators"
    Define who is eligible for BYOD. Options to consider:

    - All employees by default, after signing this policy
    - Only employees at a certain level or above
    - Case-by-case approval based on role and project requirements
    - Contractors and subconsultants allowed for email/calendar only, not project data


---

## 4. Device Requirements

Before IT will approve a personal device for firm use, it must meet these minimum requirements:

### 4.1 Laptops and Tablets

- **Operating system:** Current supported version of Windows 11, macOS, iPadOS, or ChromeOS. Devices running unsupported or end-of-life operating systems are not eligible.
- **Encryption:** Full-disk encryption enabled (BitLocker on Windows, FileVault on Mac, device encryption on tablets).
- **Screen lock:** Automatic lock after no more than 5 minutes of inactivity. PIN, password, or biometric unlock required.
- **Endpoint protection:** The firm's approved endpoint protection software must be installed if IT requires it. At minimum, built-in OS protections (Windows Defender, macOS XProtect) must be enabled and up to date.
- **Updates:** Automatic updates enabled. Security patches must be installed within 7 days of release.
- **No jailbreaking or rooting.** Devices with modified operating systems are not eligible.

### 4.2 Phones

- **Operating system:** Current or previous major version of iOS or Android.
- **Screen lock:** PIN (6+ digits), password, or biometric.
- **Encryption:** Device encryption enabled (enabled by default on modern iOS and Android).
- **Updates:** Automatic updates enabled.
- **No jailbreaking or rooting.**

### 4.3 Device Management

!!! tip "Firm administrators"
    Decide whether BYOD devices require a Mobile Device Management (MDM) profile or a lighter-touch approach:

    - **Full MDM enrollment:** IT can enforce policies, push configurations, and remotely wipe the device. Most secure, but employees may be uncomfortable with IT's level of access to a personal device.
    - **Containerized MDM:** IT manages only the work profile/container (Microsoft Intune, Google Workspace endpoint management). Personal data stays private. This is the recommended approach for most AEC firms.
    - **No MDM, policy-only:** Rely on this policy and employee attestation. Least secure, but may be the only practical option for subconsultants and short-term contractors.


---

## 5. What You Can and Can't Do on Personal Devices

### 5.1 Allowed

- Access firm email and calendar
- Join video calls and use firm messaging tools (Teams, Slack, Zoom)
- View and comment on project documents through approved cloud platforms
- Use firm-approved mobile apps for time tracking, expense reporting, and project management
- Access the firm VPN for remote work (if your device meets the requirements above)

### 5.2 Not Allowed

- Store complete BIM models, construction document sets, or project databases on personal devices
- Install firm-licensed AEC software (ArchiCAD, Revit, AutoCAD, Bluebeam, Adobe Creative Cloud) on personal devices unless IT has explicitly approved it and confirmed licensing allows it
- Sync project folders from BIM 360, Autodesk Docs, SharePoint, or BIMcloud to a personal device's local storage
- Download client files to personal cloud storage (iCloud, personal Google Drive, personal Dropbox)
- Use personal devices to access firm file servers directly (use VPN + remote desktop instead)
- Let family members or other people use a device that has access to firm resources

### 5.3 AEC-Specific Considerations

- **Large file handling:** BIM models and project files can be enormous. Don't try to sync or download large project files to personal devices with limited storage. Use Autodesk Docs, BIM 360, or Bluebeam Studio to view and mark up files in the cloud instead.
- **Licensed software:** Most AEC software licenses are assigned to specific devices or users. Using a personal device for licensed AEC software almost always requires IT involvement to manage the license correctly and ensure compliance.
- **Field work:** If you use a personal tablet or phone on project sites for photos, field observations, or punch lists, make sure project photos and notes are uploaded to the firm's approved project platform — not left sitting in your personal photo library.

---

## 6. Security Responsibilities

When you use a personal device for firm work, you're accepting these responsibilities:

1. **Keep your device secure.** Don't leave it unlocked in public places. Don't lend it to people who aren't authorized to access firm data.
2. **Report loss or theft immediately** — within 1 hour if possible. Contact IT at [INSERT IT CONTACT]. IT may need to remotely wipe firm data from the device.
3. **Don't disable security features.** If IT has installed a management profile or endpoint protection, don't remove or disable it.
4. **Separate work and personal data.** Use the work profile or container if your device supports it. Don't copy firm data into personal apps.
5. **Connect securely.** Use the firm VPN when accessing firm resources over the internet. Don't access firm email or files over public Wi-Fi without the VPN.
6. **Let IT help with issues.** If your device has a security problem (malware, suspicious behavior), tell IT. They can help without accessing your personal data in most cases.

---

## 7. Remote Wipe

If your personal device is lost, stolen, or compromised, IT may need to remotely wipe firm data from it.

- **Containerized MDM:** IT can wipe only the work profile/container. Your personal photos, messages, and apps are not affected.
- **Full MDM:** IT can perform a full device wipe if necessary. This erases everything on the device.
- **No MDM:** IT will revoke access to firm accounts (email, VPN, cloud storage) but cannot wipe data already downloaded to the device. You're responsible for deleting any firm data.

!!! tip "Firm administrators"
    Be clear about which wipe scenario applies to your BYOD program. Employees need to understand this before they enroll a personal device. If you use containerized MDM, emphasize that personal data is safe — it reduces pushback significantly.


---

## 8. Offboarding

When you leave the firm — or when your BYOD approval is revoked — the following happens:

1. IT revokes access to firm email, VPN, cloud storage, and all firm-managed applications.
2. If the device has an MDM profile, IT removes it (which may wipe the work container).
3. You must delete any firm data remaining on the device — project files, downloaded emails, cached documents, screenshots of project data.
4. Any firm-licensed software on the device must be uninstalled.

This applies regardless of whether you're leaving voluntarily or involuntarily. If you're terminated, access revocation may happen immediately — before you're notified.

---

## 9. Enforcement

- IT may verify that enrolled BYOD devices meet the requirements in this policy at any time.
- Devices that fall out of compliance (e.g., missed security updates, removed MDM profile) will have firm access revoked until the issue is resolved.
- Violations of this policy will be handled through the firm's standard disciplinary process.
- Repeated violations may result in permanent revocation of BYOD privileges.

---

## 10. Disclaimer

This policy covers the firm's requirements for personal devices used to access firm resources. It doesn't replace the firm's Acceptable Use Policy, which applies to all technology use regardless of device ownership. The firm is not responsible for damage, loss, or data loss on personal devices.

---

## 11. Acknowledgment

I have read and understand this BYOD Policy. I understand that by using my personal device for firm work, I agree to the security requirements and remote wipe provisions described in this policy.

**Name:** _______________________________________________

**Signature:** _______________________________________________

**Date:** _______________________________________________

---

## 12. Revision History

| Version | Date | Summary |
|---------|------|---------|
| 1.0 | March 2026 | Initial release |

---

*This policy is part of the [Open IT Policy Library for AEC](https://github.com/sortedsol/Open-IT-Policy-Library) by [Sorted Solution](https://www.sortedsolution.com). Free to use, fork, and adapt. Attribution appreciated.*
