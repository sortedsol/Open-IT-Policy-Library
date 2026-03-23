# IT Offboarding Checklist
**Open IT Policy Library by Sorted Solution** | [sortedsolution.com](https://www.sortedsolution.com/oitpl)<br>
*Last verified: March 2026*
*Free to use, fork, and adapt at [github.com/sortedsol/Open-IT-Policy-Library](https://github.com/sortedsol/Open-IT-Policy-Library)* | [Download DOCX version](https://github.com/sortedsol/Open-IT-Policy-Library/raw/main/policies/references/IT-Offboarding-Checklist.docx)

---

## 1. What This Is

This is a checklist for IT teams and managers to follow when someone leaves the company — whether they resign, are terminated, or a contractor's engagement ends. It covers everything from disabling accounts to recovering hardware and transferring data.

Offboarding is where most small and mid-sized companies drop the ball. A departing employee's accounts stay active for days or weeks. Their laptop sits in a drawer with client data on it. Shared passwords they knew never get rotated. Every one of these is a security risk — and some of them are compliance risks too.

This checklist makes sure nothing gets missed. The goal is simple: when someone leaves, their access ends immediately, their data is preserved for the company, and their equipment is recovered and wiped.

!!! warning "Important"
    Offboarding should start the moment a departure is confirmed — not on the employee's last day. For involuntary terminations, account disabling should happen simultaneously with the termination conversation. Coordinate with HR in advance.

!!! tip "Company administrators"
    Customize this checklist for your company's tools and environment. The companion [IT Onboarding Checklist](IT-Onboarding-Checklist.md) covers the setup process for new hires.

---

## 2. Immediate Actions (Day of Departure)

These steps should happen on the employee's last day — or, for involuntary terminations, at the time of the termination meeting. Don't wait until the next business day.

### 2.1 Account Disabling

- [ ] Disable (don't delete) the user's account in the identity provider (Microsoft Entra ID, Google Workspace, Okta, or other)
- [ ] Disable email access and set up an auto-reply or forwarding to a manager/team mailbox if needed
- [ ] Revoke VPN access
- [ ] Disable access to all SaaS and cloud platforms (see Section 3)
- [ ] Revoke any active sessions — force sign-out across all devices
- [ ] Disable MFA tokens associated with the account
- [ ] Remove the user from remote access systems (RDP, SSH, remote desktop tools)

!!! warning "Important"
    Disable accounts — don't delete them immediately. You may need the account for data retention, legal holds, or to transfer ownership of files and emails. Plan to delete accounts after a defined retention period (typically 30–90 days, depending on your policy and any legal requirements).

### 2.2 Credential Rotation

- [ ] Rotate any shared passwords the departing employee had access to (Wi-Fi passwords, shared service accounts, team-level credentials)
- [ ] Remove the departing employee from all shared vaults in the password manager
- [ ] Revoke any API keys, tokens, or service credentials the employee created or had access to
- [ ] If the employee was an IT admin, rotate all admin and service account credentials they could have known

!!! tip "Company administrators"
    Maintain a record of which shared credentials each employee has access to. If you're using a password manager with team vaults, this is straightforward — just remove them from the vaults. If shared credentials are managed informally, offboarding is a good reminder to formalize the process.

### 2.3 Hardware Recovery

- [ ] Collect the company laptop and power adapter
- [ ] Collect any other company equipment (monitors, headsets, docking stations, mice, keyboards, security keys, phones)
- [ ] If the employee worked remotely, arrange shipping with a prepaid label and tracking
- [ ] Record all returned items against the asset inventory

---

## 3. Platform and Tool Access Revocation

Disable or remove the departing employee's account from every platform they used. Don't rely on disabling the identity provider account alone — some platforms have independent logins.

### Core Platforms

- [ ] Email and calendar (Microsoft 365, Google Workspace, or other)
- [ ] File storage and sharing (SharePoint, OneDrive, Google Drive, Dropbox Business, or other)
- [ ] Chat and collaboration (Microsoft Teams, Slack, or other)
- [ ] Video conferencing (Zoom, Teams, Google Meet, or other)
- [ ] Project management (Asana, Monday, Jira, Basecamp, or other)

### Security Tools

- [ ] Password manager — remove from organization, revoke all shared vault access
- [ ] VPN — remove client certificate or user account
- [ ] MDM — initiate remote wipe of company profile from personal devices (BYOD) or full wipe of company devices
- [ ] Endpoint protection — remove device from management console (after wiping)

### Business Applications

- [ ] CRM (Salesforce, HubSpot, or other)
- [ ] Accounting / ERP (QuickBooks, Sage, or other)
- [ ] Industry-specific software (list tools relevant to your business)
- [ ] Development tools (GitHub, GitLab, Bitbucket, or other — remove from org, revoke SSH keys)
- [ ] Cloud infrastructure (AWS, Azure, GCP — remove IAM user, revoke access keys)

### External and Third-Party Access

- [ ] Client portals or systems the employee had access to — notify the client and have them revoke access
- [ ] Vendor portals and partner systems
- [ ] Social media accounts — change passwords if the employee had access
- [ ] Domain registrars, DNS management, hosting accounts — transfer ownership and change credentials

!!! tip "Company administrators"
    Replace the generic tool names above with your actual tools. Keep this list updated as you add or remove platforms. The biggest offboarding risk is the tool that nobody remembers to check.

---

## 4. Data Preservation and Transfer

### 4.1 Email

- [ ] Export or archive the departing employee's mailbox according to your retention policy
- [ ] Set up email forwarding or auto-reply for an appropriate period (typically 30–90 days)
- [ ] Transfer ownership of any shared mailboxes the employee managed

### 4.2 Files and Documents

- [ ] Transfer ownership of files in cloud storage (OneDrive, Google Drive, Dropbox) to the employee's manager or a designated team member
- [ ] Check for locally stored files on the employee's laptop before wiping — copy anything that should be preserved to company storage
- [ ] Review and transfer ownership of any shared folders or document libraries the employee created

### 4.3 Project and Business Data

- [ ] Reassign ownership of any open projects, tasks, or tickets in project management tools
- [ ] Transfer CRM account ownership (contacts, deals, pipelines)
- [ ] Redirect any automated reports, alerts, or scheduled tasks that were tied to the employee's account
- [ ] Transfer ownership of any shared calendars, bookings, or scheduling links

### 4.4 Communication History

- [ ] Determine if chat/messaging history needs to be preserved (check your retention policy and any legal hold requirements)
- [ ] Export relevant Slack, Teams, or other messaging data if required

---

## 5. Device Wiping and Redeployment

Once the laptop and any other devices are recovered:

- [ ] Back up any locally stored data that hasn't been transferred to company storage
- [ ] Verify that full-disk encryption was enabled (if not, flag this as a security concern)
- [ ] Wipe the device to factory settings
- [ ] Re-image with the company's standard software image if redeploying
- [ ] Update the asset inventory to reflect the device's new status (available, redeployed, retired)
- [ ] For BYOD devices: confirm that the company profile/data was remotely wiped via MDM

---

## 6. Involuntary Termination Considerations

Involuntary terminations require tighter coordination and faster execution.

- [ ] Coordinate with HR on the timing — IT should be ready to disable accounts at the exact time of the termination meeting
- [ ] Disable all access simultaneously: identity provider, email, VPN, remote access, and all SaaS platforms
- [ ] If the employee has a company laptop at a remote location, initiate a remote wipe via MDM immediately if there's any risk of data exfiltration
- [ ] Change any shared passwords or system credentials the employee knew before or immediately after the termination meeting
- [ ] Review recent access logs for any unusual activity (large file downloads, email forwarding rules, data exports) in the days leading up to termination

!!! warning "Important"
    For high-risk terminations (employees with admin access, employees leaving under contentious circumstances, or situations involving suspected data theft), consider engaging your managed IT provider or a security professional to assist with the offboarding and to conduct a review of recent account activity.

---

## 7. Post-Offboarding Verification

Within one week of the employee's departure, verify that offboarding is complete:

- [ ] Confirm all accounts are disabled across every platform (run through Section 3 again)
- [ ] Confirm hardware has been returned or a recovery plan is in place
- [ ] Confirm shared credentials have been rotated
- [ ] Confirm data has been transferred or archived
- [ ] Confirm email forwarding or auto-reply is active if applicable
- [ ] Check for any automated processes, scripts, or integrations that ran under the employee's account — reassign or disable them
- [ ] Remove the employee from any remaining distribution lists, security groups, and team memberships

---

## 8. Account Retention and Deletion

- [ ] Keep disabled accounts for the retention period defined by your company policy (typically 30–90 days)
- [ ] After the retention period, and after confirming no legal hold applies, permanently delete the account
- [ ] Document the deletion date in the offboarding record

!!! tip "Company administrators"
    Define your account retention period here. Check with legal counsel — some industries or contracts require longer retention. If you're subject to litigation holds, never delete accounts that may contain relevant data.

---

## 9. Offboarding Completion Sign-Off

Once all steps are complete, record the offboarding as finished.

| Field | Details |
|-------|---------|
| **Employee name** | [INSERT] |
| **Last day** | [INSERT] |
| **Department / Role** | [INSERT] |
| **Departure type** | Voluntary / Involuntary / Contract end |
| **Accounts disabled** | Yes / No |
| **Hardware returned** | Yes / No |
| **Shared credentials rotated** | Yes / No |
| **Data transferred/archived** | Yes / No |
| **Email forwarding set up** | Yes / No / N/A |
| **Completed by (IT staff)** | [INSERT] |
| **Date completed** | [INSERT] |
| **Account deletion date (scheduled)** | [INSERT] |

---

## 10. Revision History

| Version | Date | Summary |
|---------|------|---------|
| 1.0 | March 2026 | Initial release |

---

*This reference is part of the [Open IT Policy Library](https://github.com/sortedsol/Open-IT-Policy-Library) by [Sorted Solution](https://www.sortedsolution.com). Free to use, fork, and adapt. Attribution appreciated.*
