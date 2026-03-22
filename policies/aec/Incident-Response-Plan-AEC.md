# Incident Response Plan for AEC Firms
**Open IT Policy Library for AEC by Sorted Solution** | [sortedsolution.com](https://www.sortedsolution.com/oitpl)<br>
*Version 1.0 — March 2026*
*Free to use, fork, and adapt at [github.com/sortedsol/Open-IT-Policy-Library](https://github.com/sortedsol/Open-IT-Policy-Library)* | [Download DOCX version](https://github.com/sortedsol/Open-IT-Policy-Library/raw/main/policies/aec/Incident-Response-Plan-AEC.docx)

---

## 1. Purpose

This document is a starter incident response plan — a framework your firm can customize, not a finished product. It outlines the basic steps every firm should be prepared to take when a security incident occurs: a ransomware attack, a data breach, a compromised account, a lost device with project data, or any other event that threatens the firm's data or systems.

Most AEC firms don't have a dedicated security team. That's fine — but you still need a plan. When an incident happens, you don't have time to figure out who does what. This plan gives you that structure.

!!! warning "Important"
    This is a starting framework. Every firm should customize it for their specific environment, insurance requirements, and legal obligations. Have your legal counsel and insurance broker review this plan before adopting it.


---

## 2. Scope

This plan covers security incidents affecting the firm's technology systems, data, and operations. This includes:

- Ransomware or malware infections
- Unauthorized access to firm systems or accounts
- Data breaches involving client, project, or employee data
- Lost or stolen devices containing firm data
- Compromised email accounts (business email compromise)
- Phishing attacks that result in credential theft or data exposure
- Accidental data exposure (sending project data to the wrong recipient, uploading to an unapproved tool)
- Denial-of-service attacks affecting firm systems
- Insider threats (employee or contractor misusing access)

---

## 3. Incident Response Team

Every firm needs an incident response team — even if it's just three people. These are the roles, not necessarily separate people. In a small firm, one person may fill multiple roles.

### 3.1 — Core Roles

| Role | Responsibility | Who |
|------|---------------|-----|
| **Incident Lead** | Makes decisions during the incident. Coordinates the response. Communicates with leadership. | [INSERT: typically IT director or managing principal] |
| **Technical Lead** | Investigates the incident. Contains the damage. Handles technical remediation. | [INSERT: typically IT staff or managed service provider] |
| **Communications Lead** | Handles client notification, employee communication, and external inquiries. | [INSERT: typically firm principal or operations manager] |
| **Legal Advisor** | Advises on notification requirements, regulatory obligations, and liability. | [INSERT: firm's legal counsel — identify before an incident happens] |

### 3.2 — External Contacts

Fill these in now, not during an incident:

| Contact | Name / Company | Phone | Email |
|---------|---------------|-------|-------|
| Managed IT provider | [INSERT] | [INSERT] | [INSERT] |
| Cyber insurance carrier | [INSERT] | [INSERT] | [INSERT] |
| Cyber insurance breach hotline | [INSERT] | [INSERT] | [INSERT] |
| Legal counsel | [INSERT] | [INSERT] | [INSERT] |
| Incident response retainer (if applicable) | [INSERT] | [INSERT] | [INSERT] |
| FBI field office (for ransomware/major breaches) | [INSERT local field office] | [INSERT] | ic3.gov |
| State attorney general (breach notification) | [INSERT your state's AG office] | [INSERT] | [INSERT] |

!!! tip "Firm administrators"
    Fill in this table now. The single most important thing you can do to prepare for an incident is have these contacts ready. When you're in the middle of a ransomware attack at 2 AM, you don't want to be searching for your insurance broker's phone number.


---

## 4. Incident Classification

Not every security event is a full-blown incident. This classification helps you decide how to respond.

### Severity 1 — Critical

Active, confirmed compromise with immediate risk to data or operations.

Examples: active ransomware infection, confirmed data breach involving client project data, compromised admin account with evidence of unauthorized access, active business email compromise with financial fraud in progress

**Response time:** Immediate. Activate the full incident response team. Contact cyber insurance carrier.

### Severity 2 — High

Confirmed security event with potential for significant impact, but not actively causing damage right now.

Examples: compromised user account (not admin), malware detected and contained on one device, lost/stolen laptop with project data, phishing attack where credentials were entered but no unauthorized access detected yet

**Response time:** Within 2 hours. Incident Lead and Technical Lead assess and contain. Determine if escalation to Severity 1 is needed.

### Severity 3 — Medium

Suspicious activity or minor security event with limited potential impact.

Examples: suspicious email reported but no one clicked, unauthorized software found on a device, failed login attempts from unusual locations, employee reports a possible social engineering attempt

**Response time:** Within 1 business day. Technical Lead investigates. Document and resolve.

### Severity 4 — Low

Security hygiene issues or policy violations with no immediate threat.

Examples: employee using unapproved cloud storage, device with expired security software, missed security patches, minor policy violation

**Response time:** Scheduled. Address during normal operations. Document for tracking.

---

## 5. Response Phases

### Phase 1 — Detection and Reporting

**Who reports:** Anyone at the firm. Every employee should know how to report a suspected incident.

**How to report:** [INSERT IT CONTACT: email/Slack/phone]

**What to include in a report:**
- What happened (what you saw, what you did, what seems wrong)
- When it happened (as precisely as possible)
- What systems or data are affected
- Whether you clicked anything, entered credentials, or opened attachments
- Screenshots if possible

**Rule:** Report first, investigate later. Employees should never try to investigate or fix a security incident on their own. Fast reporting is not punished — delayed reporting creates real risk.

### Phase 2 — Assessment and Classification

The Incident Lead and Technical Lead assess the report:

1. Is this a real incident or a false alarm?
2. What severity level? (See Section 4)
3. What systems, data, and clients are potentially affected?
4. Is it still active or has it been contained?
5. Do we need to activate the full incident response team?
6. Do we need to contact our cyber insurance carrier? (For Severity 1 and 2: yes, immediately.)

### Phase 3 — Containment

The goal is to stop the bleeding — limit the damage without destroying evidence.

**Short-term containment (first hours):**
- Isolate affected systems from the network (disconnect, don't power off — you may need forensic data)
- Disable compromised accounts
- Block known malicious IPs, domains, or email addresses
- Preserve logs and evidence (don't delete, don't reboot if possible)
- If ransomware: disconnect affected systems from the network immediately, do NOT pay the ransom without consulting legal and insurance first

**Long-term containment (next steps):**
- Set up clean systems for critical operations if needed
- Implement temporary access restrictions
- Monitor for continued attacker activity
- Begin forensic analysis (or engage your incident response retainer)

### Phase 4 — Eradication

Remove the threat from firm systems:

- Remove malware from all affected systems
- Reset credentials for all compromised accounts (and any accounts that shared passwords)
- Patch the vulnerability that was exploited
- Verify that backups are clean before using them for restoration
- Scan all connected systems for indicators of compromise

### Phase 5 — Recovery

Restore normal operations:

- Restore systems from clean backups
- Verify that restored systems are functioning correctly
- Re-enable user access in a controlled manner
- Monitor restored systems closely for signs of reinfection
- Confirm that all project data is intact — for AEC firms, lost project data can mean lost deadlines, lost revenue, and potential professional liability

### Phase 6 — Post-Incident Review

Within 1-2 weeks of resolving the incident, conduct a review:

1. **What happened?** Timeline of the incident from detection to resolution.
2. **How did it happen?** Root cause analysis.
3. **What worked?** What parts of the response went well?
4. **What didn't work?** Where did the response break down?
5. **What needs to change?** Specific action items to prevent recurrence and improve response.
6. **Client impact?** Were any clients affected? Were notification requirements met?
7. **Insurance and legal?** Were all reporting obligations met?

Document the review. Update this plan based on lessons learned.

---

## 6. Client Notification

AEC firms have professional and contractual obligations to clients. If client data was compromised:

1. **Check contracts.** Many client contracts (especially government and institutional) have specific breach notification requirements and timelines.
2. **Consult legal counsel** before notifying clients. The language matters, and you need to understand your legal exposure before you communicate.
3. **Consult your insurance carrier.** Most cyber policies have specific requirements about how and when you notify affected parties. Some policies provide PR and legal support for notifications.
4. **Be honest but precise.** Tell clients what happened, what data was affected, what you're doing about it, and what they should do. Don't speculate about things you don't yet know.
5. **Document everything.** Every client communication about the incident should be documented.

---

## 7. State Breach Notification Requirements

Most states have laws requiring notification when personal information is breached. Requirements vary by state — notification timelines, what qualifies as "personal information," and who must be notified (individuals, state AG, credit bureaus).

!!! tip "Firm administrators"
    Identify the states where you operate and where your clients are located. Map out the breach notification requirements for each. Common requirements include:

    - Notification to affected individuals within 30-60 days (varies by state)
    - Notification to the state attorney general if the breach exceeds a certain number of records
    - Specific content requirements for notification letters

    Your legal counsel and cyber insurance carrier should help you navigate this. Don't try to figure out multi-state notification requirements during an active incident — map them out in advance.


---

## 8. Backup and Recovery Readiness

Your incident response plan is only as good as your backups. Verify the following:

- **Backup schedule:** [INSERT: e.g., daily incremental, weekly full]
- **Backup location:** [INSERT: e.g., cloud backup to Azure/AWS, offsite NAS, tape]
- **Offline/air-gapped backup:** Do you have at least one backup copy that ransomware can't reach? This is critical.
- **Recovery time:** How long does it take to restore critical systems from backup? Have you tested this?
- **What's backed up:** All project data? Email? Server configurations? Workstation images?
- **Retention:** How far back can you restore?

!!! tip "Firm administrators"
    If you haven't tested restoring from backup in the last 6 months, schedule a test. Many firms discover their backups don't actually work only when they need them.


---

## 9. Ransomware-Specific Guidance

Ransomware is the single biggest cyber threat to AEC firms. If you're hit:

1. **Disconnect affected systems from the network immediately.** Don't power them off — isolate them.
2. **Do NOT pay the ransom** without first consulting your legal counsel and cyber insurance carrier. Paying doesn't guarantee you'll get your data back, and it may violate sanctions regulations.
3. **Contact your cyber insurance carrier immediately.** Most policies have a breach hotline and will assign an incident response firm.
4. **Preserve evidence.** Don't wipe or rebuild systems until forensic analysis is complete (or until your insurance carrier's IR firm says it's okay).
5. **Report to law enforcement.** FBI's Internet Crime Complaint Center (ic3.gov) and your local FBI field office.
6. **Communicate internally.** Staff need to know what's happening and what they should and shouldn't do.
7. **Assess project deadlines.** If systems are down, which projects are at risk? Contact clients proactively about potential delays.

---

## 10. Plan Maintenance

This plan should be reviewed and updated:

- **Annually** at minimum
- **After every incident** (even minor ones)
- **When key personnel change** (especially the Incident Response Team roster)
- **When the firm's technology environment changes significantly** (new office, new cloud platform, new managed IT provider)
- **When your cyber insurance policy renews** (requirements may change)

---

## 11. Disclaimer

This incident response plan is a starting framework, not legal advice. It does not replace professional consultation with legal counsel, insurance advisors, or qualified cybersecurity professionals. Every firm should customize this plan to its specific environment, obligations, and risk profile.

---

## 12. Revision History

| Version | Date | Summary |
|---------|------|---------|
| 1.0 | March 2026 | Initial release — starter framework |

---

*This policy is part of the [Open IT Policy Library for AEC](https://github.com/sortedsol/Open-IT-Policy-Library) by [Sorted Solution](https://www.sortedsolution.com). Free to use, fork, and adapt. Attribution appreciated.*
