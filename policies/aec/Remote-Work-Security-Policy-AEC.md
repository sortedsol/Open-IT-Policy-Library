# Remote Work Security Policy for AEC Firms
**Open IT Policy Library for AEC by Sorted Solution** | [sortedsolution.com](https://www.sortedsolution.com/oitpl)<br>
*Version 1.0 — March 2026*
*Free to use, fork, and adapt at [github.com/sortedsol/Open-IT-Policy-Library](https://github.com/sortedsol/Open-IT-Policy-Library)* | [Download DOCX version](https://github.com/sortedsol/Open-IT-Policy-Library/raw/main/policies/aec/Remote-Work-Security-Policy-AEC.docx)

---

## 1. Purpose

This policy defines the security requirements for working outside the office — from home, client offices, project sites, co-working spaces, airports, hotels, and anywhere else. Remote work creates risks that don't exist in the office: unsecured networks, shared spaces, uncontrolled physical environments, and the temptation to take shortcuts.

AEC firms face additional challenges: large file transfers, bandwidth-intensive BIM workflows, field work on active construction sites, and the need to access project data from locations with unreliable internet. This policy addresses all of it.

---

## 2. Scope

This policy applies to anyone who works outside the firm's office — employees, contractors, subconsultants, and interns. It applies whether you're working from home full-time, on a hybrid schedule, visiting a project site, or working from a hotel during travel.

If you're accessing firm resources from anywhere other than the firm's office network, this policy applies to you.

---

## 3. Network Security

### 3.1 VPN Required

Always use the firm's VPN when accessing firm resources from outside the office. This includes email, cloud storage, project files, and any internal systems.

The VPN encrypts your connection so that even if the network you're on is compromised, your data stays protected. Don't access firm resources without it — even from your home network.

!!! tip "Firm administrators"
    Specify your VPN solution and enrollment process here. Include: how to install the VPN client, how to connect, who to contact if it's not working, and any split-tunneling policies.


### 3.2 Wi-Fi Security

- **Home networks:** Use WPA3 or WPA2 encryption. Change the default admin password on your router. If you're on an older router that only supports WEP, replace it or talk to IT about options.
- **Client offices and project sites:** Use the firm VPN. Don't trust the client's network, even if they say it's secure — it's not your network and you can't verify its configuration.
- **Public Wi-Fi (coffee shops, airports, hotels, co-working spaces):** Always use the firm VPN. Never access firm resources on public Wi-Fi without it. If the VPN isn't working, use your phone's mobile hotspot instead.
- **Project site trailers:** Site networks are typically unsecured. Use the firm VPN for everything. If the site doesn't have internet access, use a mobile hotspot.

### 3.3 Home Network Recommendations

Your home network doesn't need to be enterprise-grade, but it should meet a basic security standard:

- Router firmware is up to date
- Default admin credentials have been changed
- WPA3 or WPA2 encryption is enabled
- The network name (SSID) doesn't identify you or the firm
- IoT devices (smart speakers, cameras, thermostats) are on a separate network or VLAN if your router supports it — these devices are often poorly secured and can be a gateway into your network

!!! tip "Firm administrators"
    Decide whether you want IT to provide a recommended home router configuration, or whether employees are responsible for their own home networks. Some firms provide a stipend for home office equipment, which can include a quality router.


---

## 4. Device Security

Every device used for remote work must meet these requirements:

- **Encryption:** Full-disk encryption enabled (BitLocker on Windows, FileVault on Mac).
- **Screen lock:** Automatic lock after no more than 5 minutes of inactivity.
- **Updates:** Operating system and applications kept current. Security patches installed within 7 days of release.
- **Endpoint protection:** The firm's approved endpoint protection software installed and running.
- **Firmware:** BIOS/UEFI password set if the device will be used regularly outside the office.

If you're using a personal device for firm work, the BYOD Policy also applies.

---

## 5. Physical Security

### 5.1 Home Office

- Work in a private area when handling confidential client data. If you're on a video call discussing a project, make sure your screen isn't visible to people who shouldn't see it.
- Lock your workstation when you step away, even at home. If other people live with you, they shouldn't have casual access to firm data on your screen.
- Don't print confidential project documents at home unless you have a way to securely dispose of them (shredder). Don't throw client drawings or specifications in your household trash or recycling.

### 5.2 Travel and Public Spaces

- Never leave a firm laptop unattended in a car, hotel room (unless in a safe), conference room, or airport.
- Use a privacy screen on your laptop when working in public spaces — especially on planes and in co-working spaces.
- Don't discuss confidential client or project information on phone calls in public places where you can be overheard. This includes airport gates, coffee shops, and shared co-working areas.
- When working from a client's office, follow their physical security requirements in addition to the firm's.

### 5.3 Project Sites

- Personal devices and laptops on active construction sites face additional physical risks (dust, water, theft from site trailers). Take appropriate precautions.
- Don't leave devices unattended in site trailers, especially on sites with multiple subcontractors and vendors coming and going.
- If you use a tablet for field observations, punch lists, or site photos, make sure it's configured for remote wipe in case of loss or theft.

---

## 6. Data Handling While Remote

### 6.1 Cloud-First

When working remotely, use the firm's cloud platforms (BIM 360, Autodesk Docs, SharePoint, OneDrive, Bluebeam Studio, BIMcloud) to access and collaborate on project files. Don't download large file sets to your local machine unless you need to work offline.

### 6.2 Offline Work

If you need to work offline (e.g., on a flight, at a site with no connectivity):

- Sync only the specific files you need, not entire project folders.
- Make sure your device is encrypted.
- Sync your changes back to the firm's cloud platform as soon as you're back online.
- Don't leave offline copies of project data on your device longer than necessary.

### 6.3 File Transfers

- Don't email project files to personal email addresses so you can access them from a personal device. Use the firm's approved cloud sharing methods.
- Don't use personal cloud storage (Google Drive, iCloud, personal Dropbox) to transfer or store project files.
- Don't use USB drives for file transfer unless IT has approved it for a specific purpose.

---

## 7. Video Conferencing and Screen Sharing

- Before sharing your screen on a video call, close or minimize any windows with confidential client data, personal information, or other projects that the call participants shouldn't see.
- Be aware of what's visible behind you on camera — whiteboards, sticky notes, and printed project documents can reveal confidential information.
- Use the firm's approved video conferencing tools. Don't use personal Zoom/Google Meet accounts for client calls.
- When recording meetings, follow the firm's recording policy and make sure all participants are aware they're being recorded.

---

## 8. Incident Reporting While Remote

The same incident reporting requirements apply whether you're in the office or working remotely. If something goes wrong — lost device, suspicious email, possible security breach — report it to IT immediately.

**How to report:** [INSERT IT CONTACT: email/Slack/phone]

Remote incidents can be harder for IT to respond to, so fast reporting is even more important. If your laptop is stolen from a site trailer on a Friday afternoon, IT needs to know right away — not Monday morning.

!!! tip "Firm administrators"
    Insert your actual IT contact method above. Consider whether you need a separate after-hours contact for remote incident reporting.


---

## 9. Bandwidth and Performance

### 9.1 Large Files

AEC workflows often involve large files — BIM models, point clouds, rendering outputs, full construction document sets. Working with these files over a remote connection can be slow and frustrating.

- Use cloud-native tools (Autodesk Docs, BIM 360, Bluebeam Studio) when possible — they're designed for remote collaboration on large files.
- For CAD/BIM work that requires local processing power, consider using a remote desktop connection to a firm workstation rather than trying to sync large files over a home connection.
- Don't sync entire project folders to your local machine. Sync only what you need.

### 9.2 Internet Requirements

!!! tip "Firm administrators"
    Consider publishing minimum internet speed recommendations for remote workers. A reasonable baseline for AEC work: 50 Mbps download / 10 Mbps upload for general office work, 100+ Mbps for BIM-heavy workflows. Consider offering a stipend for employees who need to upgrade their home internet.


---

## 10. Enforcement

- IT may verify that remote devices and configurations meet this policy's requirements.
- Devices that don't meet the requirements will have remote access revoked until the issue is resolved.
- Violations will be handled through the firm's standard disciplinary process.

---

## 11. Disclaimer

This policy covers the firm's requirements for working outside the office. It doesn't replace the firm's Acceptable Use Policy, BYOD Policy, or project-specific security requirements. If a client contract imposes stricter remote work requirements, the stricter requirement applies.

---

## 12. Acknowledgment

I have read and understand this Remote Work Security Policy. I understand that I am responsible for maintaining the security of firm data and devices when working outside the office.

**Name:** _______________________________________________

**Signature:** _______________________________________________

**Date:** _______________________________________________

---

## 13. Revision History

| Version | Date | Summary |
|---------|------|---------|
| 1.0 | March 2026 | Initial release |

---

*This policy is part of the [Open IT Policy Library for AEC](https://github.com/sortedsol/Open-IT-Policy-Library) by [Sorted Solution](https://www.sortedsolution.com). Free to use, fork, and adapt. Attribution appreciated.*
