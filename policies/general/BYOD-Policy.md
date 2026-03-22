# BYOD Policy
**Open IT Policy Library by Sorted Solution** | [sortedsolution.com](https://www.sortedsolution.com/oitpl)<br>
*Version 1.0 — March 2026*
*Free to use, fork, and adapt at [github.com/sortedsol/Open-IT-Policy-Library](https://github.com/sortedsol/Open-IT-Policy-Library)* | [Download DOCX version](https://github.com/sortedsol/Open-IT-Policy-Library/raw/main/policies/general/BYOD-Policy.docx)

---

## 1. Purpose

This policy defines the rules for using personal devices — laptops, tablets, and phones — to access the company's network, email, files, and applications. "BYOD" stands for Bring Your Own Device.

This policy balances the flexibility employees want with the security the company and its clients require.

---

## 2. Scope

This policy applies to anyone who uses a personally owned device to access the company's resources — employees, contractors, consultants, and interns.

"Company resources" includes:

- Company email (Microsoft 365, Google Workspace)
- Cloud storage and collaboration platforms (SharePoint, OneDrive, Dropbox, Google Drive, Slack, Teams)
- The company's VPN
- Company-managed applications and project management tools
- Any system you log into with company credentials

This policy does **not** cover company-owned devices that employees take home — those are covered by the company's Acceptable Use Policy.

---

## 3. Who Can Use Personal Devices

BYOD is not automatic. You need IT approval before using a personal device for company work.

> **Companies:** Define who is eligible for BYOD. Options to consider:
>
> - All employees by default, after signing this policy
> - Only employees at a certain level or above
> - Case-by-case approval based on role
> - Contractors allowed for email/calendar only, not client data

---

## 4. Device Requirements

Before IT will approve a personal device for company use, it must meet these minimum requirements:

### 4.1 — Laptops and Tablets

- **Operating system:** Current supported version of Windows 11, macOS, iPadOS, or ChromeOS. Devices running unsupported or end-of-life operating systems are not eligible.
- **Encryption:** Full-disk encryption enabled (BitLocker on Windows, FileVault on Mac, device encryption on tablets).
- **Screen lock:** Automatic lock after no more than 5 minutes of inactivity. PIN, password, or biometric unlock required.
- **Endpoint protection:** The company's approved endpoint protection software must be installed if IT requires it. At minimum, built-in OS protections (Windows Defender, macOS XProtect) must be enabled and up to date.
- **Updates:** Automatic updates enabled. Security patches must be installed within 7 days of release.
- **No jailbreaking or rooting.** Devices with modified operating systems are not eligible.

### 4.2 — Phones

- **Operating system:** Current or previous major version of iOS or Android.
- **Screen lock:** PIN (6+ digits), password, or biometric.
- **Encryption:** Device encryption enabled (enabled by default on modern iOS and Android).
- **Updates:** Automatic updates enabled.
- **No jailbreaking or rooting.**

### 4.3 — Device Management

> **Companies:** Decide whether BYOD devices require a Mobile Device Management (MDM) profile or a lighter-touch approach:
>
> - **Full MDM enrollment:** IT can enforce policies, push configurations, and remotely wipe the device. Most secure, but employees may be uncomfortable with IT's level of access to a personal device.
> - **Containerized MDM:** IT manages only the work profile/container (Microsoft Intune, Google Workspace endpoint management). Personal data stays private. This is the recommended approach for most companies.
> - **No MDM, policy-only:** Rely on this policy and employee attestation. Least secure, but may be the only practical option for short-term contractors.

---

## 5. What You Can and Can't Do on Personal Devices

### 5.1 — Allowed

- Access company email and calendar
- Join video calls and use company messaging tools (Teams, Slack, Zoom)
- View and comment on documents through approved cloud platforms
- Use company-approved mobile apps for time tracking, expense reporting, and project management
- Access the company VPN for remote work (if your device meets the requirements above)

### 5.2 — Not Allowed

- Store client databases, complete project archives, or bulk data exports on personal devices
- Install company-licensed software on personal devices unless IT has explicitly approved it
- Sync work folders from SharePoint, OneDrive, or company cloud storage to a personal device's local storage
- Download client files to personal cloud storage (iCloud, personal Google Drive, personal Dropbox)
- Use personal devices to access company file servers directly (use VPN + remote desktop instead)
- Let family members or other people use a device that has access to company resources

---

## 6. Security Responsibilities

When you use a personal device for company work, you're accepting these responsibilities:

1. **Keep your device secure.** Don't leave it unlocked in public places. Don't lend it to people who aren't authorized to access company data.
2. **Report loss or theft immediately** — within 1 hour if possible. Contact IT at [INSERT IT CONTACT]. IT may need to remotely wipe company data from the device.
3. **Don't disable security features.** If IT has installed a management profile or endpoint protection, don't remove or disable it.
4. **Separate work and personal data.** Use the work profile or container if your device supports it. Don't copy company data into personal apps.
5. **Connect securely.** Use the company VPN when accessing company resources over the internet. Don't access company email or files over public Wi-Fi without the VPN.
6. **Let IT help with issues.** If your device has a security problem (malware, suspicious behavior), tell IT. They can help without accessing your personal data in most cases.

---

## 7. Remote Wipe

If your personal device is lost, stolen, or compromised, IT may need to remotely wipe company data from it.

- **Containerized MDM:** IT can wipe only the work profile/container. Your personal photos, messages, and apps are not affected.
- **Full MDM:** IT can perform a full device wipe if necessary. This erases everything on the device.
- **No MDM:** IT will revoke access to company accounts (email, VPN, cloud storage) but cannot wipe data already downloaded to the device. You're responsible for deleting any company data.

> **Companies:** Be clear about which wipe scenario applies to your BYOD program. Employees need to understand this before they enroll a personal device. If you use containerized MDM, emphasize that personal data is safe — it reduces pushback significantly.

---

## 8. Offboarding

When you leave the company — or when your BYOD approval is revoked — the following happens:

1. IT revokes access to company email, VPN, cloud storage, and all company-managed applications.
2. If the device has an MDM profile, IT removes it (which may wipe the work container).
3. You must delete any company data remaining on the device — client files, downloaded emails, cached documents.
4. Any company-licensed software on the device must be uninstalled.

This applies regardless of whether you're leaving voluntarily or involuntarily. If you're terminated, access revocation may happen immediately — before you're notified.

---

## 9. Enforcement

- IT may verify that enrolled BYOD devices meet the requirements in this policy at any time.
- Devices that fall out of compliance (e.g., missed security updates, removed MDM profile) will have company access revoked until the issue is resolved.
- Violations of this policy will be handled through the company's standard disciplinary process.
- Repeated violations may result in permanent revocation of BYOD privileges.

---

## 10. Disclaimer

This policy covers the company's requirements for personal devices used to access company resources. It doesn't replace the company's Acceptable Use Policy, which applies to all technology use regardless of device ownership. The company is not responsible for damage, loss, or data loss on personal devices.

---

## 11. Acknowledgment

I have read and understand this BYOD Policy. I understand that by using my personal device for company work, I agree to the security requirements and remote wipe provisions described in this policy.

**Name:** _______________________________________________

**Signature:** _______________________________________________

**Date:** _______________________________________________

---

## 12. Revision History

| Version | Date | Summary |
|---------|------|---------|
| 1.0 | March 2026 | Initial release |

---

*This policy is part of the [Open IT Policy Library](https://github.com/sortedsol/Open-IT-Policy-Library) by [Sorted Solution](https://www.sortedsolution.com). Free to use, fork, and adapt. Attribution appreciated.*
