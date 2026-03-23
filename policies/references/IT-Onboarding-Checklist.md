# IT Onboarding Checklist
**Open IT Policy Library by Sorted Solution** | [sortedsolution.com](https://www.sortedsolution.com/oitpl)<br>
*Last verified: March 2026*
*Free to use, fork, and adapt at [github.com/sortedsol/Open-IT-Policy-Library](https://github.com/sortedsol/Open-IT-Policy-Library)* | [Download DOCX version](https://github.com/sortedsol/Open-IT-Policy-Library/raw/main/policies/references/IT-Onboarding-Checklist.docx)

---

## 1. What This Is

This is a checklist for IT teams and managers to follow when a new employee, contractor, or consultant starts. It covers everything from account creation to security training — the full set of steps needed to get someone set up securely and productively on day one.

Most small and mid-sized companies don't have a formal onboarding process for IT. New hires get a laptop and an email address, and the rest happens ad hoc over the first week (or month). That's how people end up with too much access, no MFA, and no idea where to find the tools they need.

This checklist fixes that. Customize it for your company's tools and environment, then use it every time someone joins.

!!! tip "Company administrators"
    This checklist is a starting template. Go through it once and fill in the specifics for your company — your tools, your platforms, your policies. Then use it as a repeatable process for every new hire. The companion [IT Offboarding Checklist](IT-Offboarding-Checklist.md) covers the reverse process when someone leaves.

---

## 2. Pre-Start Setup

Complete these before the new hire's first day.

### Hardware

- [ ] Order and configure laptop (company-managed, with full-disk encryption enabled)
- [ ] Set up peripheral equipment if needed (monitor, keyboard, mouse, docking station, headset)
- [ ] Apply asset tag and record serial number, model, and assigned user in the asset inventory
- [ ] Install the company's standard software image or baseline applications

!!! tip "Company administrators"
    List your standard hardware configuration here — laptop models, monitor specs, and any role-specific equipment (e.g., high-performance workstations for CAD users, dual monitors for project managers). Include where to order from and typical lead times.

### Accounts and Access

- [ ] Create email account and configure email signature template
- [ ] Create account in the identity provider (Microsoft Entra ID, Google Workspace, Okta, or other)
- [ ] Assign to appropriate security groups and distribution lists based on role and department
- [ ] Create accounts in company-approved platforms and tools (see Section 3)
- [ ] Set up VPN access if the role involves remote work
- [ ] Generate temporary credentials and prepare a secure method to deliver them to the new hire

!!! tip "Company administrators"
    Specify your identity provider and standard security groups here. Include a list of groups by department or role so IT doesn't have to guess which groups a new marketing hire should be in versus a new engineer.

### Workspace

- [ ] Assign phone extension or softphone license if applicable
- [ ] Set up physical workspace (desk, chair, power, network drop) if in-office
- [ ] Prepare welcome packet with IT contact information and links to key resources

---

## 3. Standard Software and Platforms

Install and configure access to the company's standard tools. Check off each one as the account is created and the software is installed.

### Core Productivity

- [ ] Email and calendar (Microsoft 365, Google Workspace, or other)
- [ ] File storage and sharing (SharePoint, OneDrive, Google Drive, Dropbox Business, or other)
- [ ] Office suite (Microsoft Office, Google Docs, or other)
- [ ] Chat and collaboration (Microsoft Teams, Slack, or other)
- [ ] Video conferencing (Zoom, Teams, Google Meet, or other)

### Security Tools

- [ ] Endpoint protection / antivirus (specify your tool)
- [ ] Password manager (1Password, Bitwarden, Keeper, or other — company-managed account)
- [ ] VPN client installed and configured
- [ ] MFA enrolled on the new hire's primary account (see MFA setup in Section 5)

### Role-Specific Tools

- [ ] Project management (Asana, Monday, Jira, Basecamp, or other)
- [ ] CRM (Salesforce, HubSpot, or other)
- [ ] Accounting / ERP (QuickBooks, Sage, or other)
- [ ] Industry-specific software (list tools relevant to your business)
- [ ] Development tools (GitHub, VS Code, or other — if applicable)

!!! tip "Company administrators"
    Replace the generic tool names above with your actual tools. If you have role-based tool lists (e.g., all project managers get Asana and Bluebeam, all designers get Adobe Creative Cloud), document those here so IT can configure the right set of tools without asking the hiring manager every time.

---

## 4. Security Configuration

### 4.1 MFA Enrollment

- [ ] Enroll the new hire in multi-factor authentication on their primary account before they access any company resources
- [ ] Preferred method: authenticator app (Microsoft Authenticator, Google Authenticator, or other) with number matching enabled, or hardware security key for admin/executive roles
- [ ] Register a backup MFA method (backup codes, secondary device, or backup hardware key)
- [ ] Verify MFA is working before proceeding with the rest of onboarding

For guidance on choosing MFA methods, see the [MFA Method Comparison](MFA-Method-Comparison.md).

### 4.2 Password Manager Setup

- [ ] Create the new hire's account in the company password manager
- [ ] Share any team or department password vaults they need access to
- [ ] Walk them through creating a strong master password (see [Password Policy Best Practices](Password-Policy-Best-Practices.md))
- [ ] Show them how to generate and store unique passwords for each service

### 4.3 Device Security Verification

- [ ] Full-disk encryption enabled and confirmed (BitLocker on Windows, FileVault on Mac)
- [ ] Automatic screen lock set to 5 minutes or less
- [ ] Endpoint protection installed and reporting to the management console
- [ ] Operating system and all applications fully patched
- [ ] BIOS/UEFI password set (if the role involves regular off-site work)
- [ ] Device enrolled in mobile device management (MDM) if applicable

---

## 5. Permissions and Access Levels

### 5.1 Principle of Least Privilege

Give the new hire access to what they need for their role — nothing more. It's much easier to grant additional access later than to clean up over-provisioned accounts.

- [ ] Review the role's required access with the hiring manager
- [ ] Assign permissions based on role, not by copying another user's access (another user may have accumulated permissions over time that aren't appropriate for the new role)
- [ ] Document what access was granted and why

### 5.2 Admin Access

- [ ] If the role requires admin access to any system, document the justification
- [ ] Admin accounts should use phishing-resistant MFA (hardware key or device-bound passkey)
- [ ] If possible, set up a separate admin account rather than granting admin rights to the user's daily account

### 5.3 Shared Resources

- [ ] Grant access to relevant shared drives, folders, and document libraries
- [ ] Grant access to shared mailboxes or distribution lists if applicable
- [ ] Grant access to shared credentials in the password manager (team vaults only — not individual credentials)

---

## 6. Policy Acknowledgment

The new hire should read and sign the following policies during their first week. Provide copies and collect signed acknowledgments.

- [ ] Acceptable Use Policy
- [ ] AI Acceptable Use Policy
- [ ] BYOD Policy (if they'll use personal devices for work)
- [ ] Remote Work Security Policy (if they'll work remotely)
- [ ] Any client-specific security requirements relevant to their role

!!! tip "Company administrators"
    List the exact policies your company requires new hires to sign, and specify where signed copies are stored (HR file, SharePoint folder, etc.). If you use the policies from this library, link directly to your customized versions.

---

## 7. Security Awareness Training

- [ ] Schedule or assign security awareness training to be completed within the first two weeks
- [ ] Topics should include: phishing recognition, password hygiene, MFA usage, acceptable use, data handling, and incident reporting
- [ ] Record training completion date

!!! tip "Company administrators"
    Specify your training platform (KnowBe4, Proofpoint Security Awareness, Ninjio, or other) and the specific training modules new hires are required to complete. If you don't have a formal platform, consider scheduling a 30-minute walkthrough with IT covering the basics.

---

## 8. Day One Walkthrough

On the new hire's first day, walk them through:

- [ ] How to log in and use MFA
- [ ] How to connect to the VPN (if applicable)
- [ ] Where to find files and shared resources
- [ ] How to use the company chat/collaboration platform
- [ ] How to reach IT for support (help desk email, Slack channel, phone)
- [ ] How to report a security incident (who to contact and how)
- [ ] Where to find company IT policies

This doesn't need to be a formal training session — a 20-minute screen share or sit-down with IT is enough to make sure the new hire isn't lost on day one.

---

## 9. Onboarding Completion Sign-Off

Once all steps are complete, record the onboarding as finished.

| Field | Details |
|-------|---------|
| **Employee name** | [INSERT] |
| **Start date** | [INSERT] |
| **Department / Role** | [INSERT] |
| **Laptop serial number** | [INSERT] |
| **Accounts created** | [LIST: email, identity provider, VPN, password manager, etc.] |
| **MFA enrolled** | Yes / No |
| **Policies signed** | Yes / No |
| **Security training assigned** | Yes / No |
| **Completed by (IT staff)** | [INSERT] |
| **Date completed** | [INSERT] |

---

## 10. Revision History

| Version | Date | Summary |
|---------|------|---------|
| 1.0 | March 2026 | Initial release |

---

*This reference is part of the [Open IT Policy Library](https://github.com/sortedsol/Open-IT-Policy-Library) by [Sorted Solution](https://www.sortedsolution.com). Free to use, fork, and adapt. Attribution appreciated.*
