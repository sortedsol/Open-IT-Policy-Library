# Password Policy Best Practice Tracker
**Open IT Policy Library by Sorted Solution** | [sortedsolution.com](https://www.sortedsolution.com/oitpl)<br>
*Last verified: March 2026*
*Free to use, fork, and adapt at [github.com/sortedsol/Open-IT-Policy-Library](https://github.com/sortedsol/Open-IT-Policy-Library)* | [Download DOCX version](https://github.com/sortedsol/Open-IT-Policy-Library/raw/main/policies/references/Password-Policy-Best-Practices.docx)

---

## 1. What This Is

This is a living reference page — not a policy template. It tracks the current password and authentication guidance from three major authorities side by side, so you can build or update your company's password policy based on what the experts actually recommend today.

If your company still requires password changes every 90 days, forces uppercase-lowercase-number-symbol complexity, or doesn't use MFA — this page will show you how far behind current best practices you've fallen, and exactly what the authorities say to do instead.

---

## 2. The Big Three: Current Guidance at a Glance

| Recommendation | NIST SP 800-63B (Rev 4) | Microsoft (Entra ID / M365) | CIS Controls v8 + CIS Password Guide |
|---|---|---|---|
| **Minimum password length** | 15 characters (no MFA) / 8 characters (with MFA) | 8 characters (system minimum, not customizable); **14 characters recommended** | 14 characters (no MFA) / 8 characters (with MFA) |
| **Complexity rules** (uppercase, symbols, etc.) | **None.** Explicitly rejects composition rules. Length is the primary strength factor. | 3 of 4 categories required (uppercase, lowercase, numbers, symbols). **Not customizable** in Entra ID. | None for MFA-enabled accounts. For password-only: a number or special character is recommended but not rigidly required. |
| **Mandatory password rotation** | **No.** Only change if evidence of compromise. | **No.** Passwords set to "never expire" by default and recommended. | **No.** Only change if evidence of compromise. Prevent rapid changes (24-hour minimum between changes). |
| **MFA required?** | Encouraged at AAL1. Mandatory at AAL2 and above. | Mandatory for Azure portal access as of October 2026. Security Defaults (which includes MFA) enabled by default for new tenants. | Strongly recommended. Recognized as the "most secure user authentication method available." |
| **Banned / blocked passwords** | Required. Must block commonly used, expected, and breached passwords. | Built in. Global banned list + customizable list (up to 1,000 terms). Checked at creation, change, and reset. | Required. Block bad, breached, and organization-specific passwords. |
| **Maximum password length** | Support at least 64 characters. | 256 characters. | No explicit maximum specified. Support long passphrases. |
| **Passphrases** | Encouraged. Long, memorable phrases are stronger than short complex passwords. | Supported but not specifically promoted. | Explicitly recommended over traditional passwords. |
| **Password managers** | Supported. Allow paste in password fields. | Not explicitly addressed in policy docs. | Recommended. |
| **Account lockout** | Not explicitly specified; rate limiting recommended. | 10 failed attempts → 1-minute Smart Lockout. | 5 failed attempts → lockout (duration at company discretion). |
| **Session timeout** | Based on risk assessment. | Configurable via Conditional Access. | 15 minutes of inactivity. |

---

## 3. What This Means for Your Company

### Stop doing these things

- **Stop requiring password changes every 30, 60, or 90 days.** All three authorities agree: mandatory rotation causes people to pick weaker passwords and increment them predictably (Password1, Password2, Password3...). Only force a change when there's evidence of compromise.
- **Stop requiring uppercase-lowercase-number-symbol complexity** (unless you're locked into Microsoft's Entra ID defaults, which you can't change — but don't stack additional complexity rules on top). NIST and CIS are clear: length beats complexity. A 20-character passphrase is far stronger than an 8-character password with special characters.
- **Stop allowing short passwords.** If you're still accepting 8-character passwords without MFA, every authority says you're below the minimum acceptable standard.

### Start doing these things

- **Enforce MFA everywhere you can.** This is the single most impactful thing you can do. All three authorities agree. Start with admin accounts, then roll it out to all users. Microsoft is making it mandatory for Azure portal access in late 2026.
- **Use a banned password list.** Block the passwords that attackers try first — common passwords, breached passwords, and passwords based on your company name, city, or industry terms. Microsoft includes this in Entra ID. For other systems, tools like "Have I Been Pwned" provide breach datasets.
- **Encourage passphrases.** "correct horse battery staple" is easier to remember and harder to crack than "P@ssw0rd!". Encourage employees to use passphrases — 4-5 random words strung together.
- **Support password managers.** Don't block paste in password fields. Encourage employees to use a password manager so they can maintain unique, long passwords for every service.
- **Set your minimum to at least 14 characters** for any account that doesn't have MFA. If MFA is enabled, 8 characters is acceptable per NIST and CIS, but 14+ is still better.

### The Microsoft complexity problem

There's a well-known tension between NIST/CIS guidance and Microsoft's implementation. NIST and CIS say **don't require complexity rules** — just enforce length. But Microsoft Entra ID (Azure AD) has **fixed, non-customizable complexity requirements**: passwords must include 3 of 4 character categories. You can't turn this off.

This isn't a reason to skip MFA or other improvements. Work within Microsoft's constraints and focus on what you can control: minimum length (push for 14+), MFA enforcement, banned password lists, and eliminating mandatory rotation. The complexity requirement is a minor annoyance, not a dealbreaker.

---

## 4. Recommended Baseline for SMBs

Based on the consensus across all three authorities, here's a practical baseline for small and mid-sized businesses:

| Setting | Recommendation |
|---------|---------------|
| Minimum password length | 14 characters (12 absolute minimum with MFA) |
| Complexity rules | Follow your platform's defaults. Don't add extra rules beyond what the system requires. |
| Password expiration | Never expire. Change only on evidence of compromise. |
| MFA | Required for all users, all applications. Phishing-resistant MFA (FIDO2, passkeys) preferred when available. |
| Banned passwords | Enable your platform's built-in banned password list. Add company-specific terms. |
| Account lockout | 5-10 failed attempts → lockout for 15-30 minutes. |
| Password manager | Recommended and supported. Provide a company-managed option if budget allows. |
| Passphrases | Encouraged. Train employees on how to create good ones. |
| Password reuse | Block reuse of at least the last 10 passwords. |

---

## 5. Sources and Further Reading

### NIST

- [NIST SP 800-63B Revision 4 — Digital Identity Guidelines: Authentication and Lifecycle Management](https://pages.nist.gov/800-63-4/sp800-63b.html)

### Microsoft

- [Microsoft 365 Password Policy Recommendations](https://learn.microsoft.com/en-us/microsoft-365/admin/misc/password-policy-recommendations)
- [Set Password Expiration Policy for Microsoft 365](https://learn.microsoft.com/en-us/microsoft-365/admin/manage/set-password-expiration-policy)
- [Microsoft Entra ID Combined Password Policy](https://learn.microsoft.com/en-us/entra/identity/authentication/concept-password-ban-bad-combined-policy)

### CIS

- [CIS Password Policy Guide](https://www.cisecurity.org/insights/white-papers/cis-password-policy-guide)
- [CIS Controls v8 — Control 5.2: Use Unique Passwords](https://controls-assessment-specification.readthedocs.io/en/latest/control-5/control-5.2.html)

---

## 6. Revision History

| Version | Date | Summary |
|---------|------|---------|
| 1.0 | March 2026 | Initial release — NIST Rev 4, Microsoft Entra ID, CIS Controls v8 |

---

*This reference is part of the [Open IT Policy Library](https://github.com/sortedsol/Open-IT-Policy-Library) by [Sorted Solution](https://www.sortedsolution.com). Free to use, fork, and adapt. Attribution appreciated.*
