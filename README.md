# Open IT Policy Library
**by [Sorted Solution](https://www.sortedsolution.com)** | [sortedsolution.com/oitpl](https://www.sortedsolution.com/oitpl)

Practical, enforceable IT policies written for small and mid-sized professional services firms — with a dedicated track for Architecture, Engineering, and Construction (AEC) firms.

---

## What This Is

This is a free, open-source library of IT policy templates designed for firms that actually need to implement them — not just check a compliance box. Every policy in this library:

- Names specific tools, platforms, and configurations instead of using vague "approved software" language
- Includes enforcement hooks so IT can actually audit and enforce each requirement
- Contains clearly marked `Firms:` sections where your organization customizes the policy to match your tools, contracts, and risk tolerance
- Is written for employees, contractors, and subconsultants — ready to drop into an employee handbook without rewriting the tone

## Who This Is For

**Track 1 — General SMB:** Any small or mid-sized professional services firm that needs real IT governance documents without hiring a consultant to write them from scratch.

**Track 2 — AEC Firms:** Architecture, engineering, and construction firms running industry-standard tools (ArchiCAD, Revit, AutoCAD, Bluebeam, M365, Google Workspace, Adobe Creative Cloud). These policies reference the actual software stack AEC firms use, with AEC-specific data classifications and risk scenarios.

## Repository Structure

```
Open-IT-Policy-Library/
├── README.md
├── policies/
│   ├── aec/                    ← AEC-specific policies
│   │   ├── AI-Acceptable-Use-Policy-AEC.md
│   │   ├── Acceptable-Use-Policy-AEC.md
│   │   ├── BYOD-Policy-AEC.md
│   │   ├── Remote-Work-Security-Policy-AEC.md
│   │   └── Incident-Response-Plan-AEC.md
│   ├── general/                ← General SMB policies
│   │   ├── AI-Acceptable-Use-Policy.md
│   │   ├── Acceptable-Use-Policy.md
│   │   ├── BYOD-Policy.md
│   │   ├── Remote-Work-Security-Policy.md
│   │   └── Incident-Response-Plan.md
│   └── references/             ← Shared reference documents
│       └── Password-Policy-Best-Practices.md
```

## Current Policies

### AEC Track

| Policy | Status | Description |
|--------|--------|-------------|
| [AI Acceptable Use Policy for AEC Firms](policies/aec/AI-Acceptable-Use-Policy-AEC.md) | Published | Four-tier AI tool classification, AEC data classification, vendor-specific guidance with DPA links, incident response, and enforcement hooks. |
| [Acceptable Use Policy for AEC Firms](policies/aec/Acceptable-Use-Policy-AEC.md) | Published | Technology acceptable use covering AEC software licensing, BIM file management, data handling, network use, and physical security. |
| [BYOD Policy for AEC Firms](policies/aec/BYOD-Policy-AEC.md) | Published | Personal device requirements, AEC-specific restrictions on BIM data and licensed software, MDM options, remote wipe, and offboarding. |
| [Remote Work Security Policy for AEC Firms](policies/aec/Remote-Work-Security-Policy-AEC.md) | Published | VPN requirements, Wi-Fi security, project site considerations, large file handling, physical security for remote and field work. |
| [Incident Response Plan for AEC Firms](policies/aec/Incident-Response-Plan-AEC.md) | Published | Starter IR framework with severity classification, response phases, ransomware guidance, client notification, and contact roster template. |

### General SMB Track

| Policy | Status | Description |
|--------|--------|-------------|
| [AI Acceptable Use Policy](policies/general/AI-Acceptable-Use-Policy.md) | Published | Four-tier AI tool classification, data classification, vendor-specific guidance with DPA links, incident response, and enforcement hooks — written for any professional services firm. |
| [Acceptable Use Policy](policies/general/Acceptable-Use-Policy.md) | Published | Technology acceptable use covering software licensing, cloud storage, data handling, network use, and physical security. |
| [BYOD Policy](policies/general/BYOD-Policy.md) | Published | Personal device requirements, MDM options, remote wipe provisions, security responsibilities, and offboarding. |
| [Remote Work Security Policy](policies/general/Remote-Work-Security-Policy.md) | Published | VPN requirements, Wi-Fi security, home network recommendations, physical security, and data handling for remote workers. |
| [Incident Response Plan](policies/general/Incident-Response-Plan.md) | Published | Starter IR framework with severity classification, response phases, ransomware guidance, client notification, and contact roster template. |

### Shared References

| Document | Status | Description |
|----------|--------|-------------|
| [Password Policy Best Practice Tracker](policies/references/Password-Policy-Best-Practices.md) | Published | Side-by-side comparison of current NIST, Microsoft, and CIS password and authentication guidance. Replaces outdated "change every 90 days" advice. |

## How to Use These Policies

1. **Fork or download** the policy you need.
2. **Search for `Firms:` sections** — these are clearly marked blocks where you need to customize the policy for your organization (insert your IT contact info, adjust tool lists to match your subscriptions, define review requirements for your practice areas).
3. **Search for `[INSERT` placeholders** — a few fields require your firm-specific information.
4. **Review with your leadership and legal counsel** before adding to your employee handbook. These policies are templates, not legal advice.
5. **Keep the attribution header** — it helps other firms find these resources. The header includes a link back to this repository and to Sorted Solution.

## How to Contribute

Contributions are welcome. If you have improvements, corrections, or new policy suggestions:

1. **Open an issue** to discuss the change before submitting a pull request.
2. **Pull requests** should include a clear description of what changed and why.
3. **Vendor-specific claims** (data handling, licensing, DPA terms) must include a link to the vendor's current documentation. We do not accept unverified vendor claims.
4. **Tone and audience:** All policies are written for employees, contractors, and subconsultants — not for firm owners or IT administrators (except in clearly marked `Firms:` sections). Maintain this voice in contributions.
5. **No proprietary content:** Do not submit policies that contain your firm's confidential information, client names, or internal procedures.

## Attribution

Every policy in this library carries a header attributing it to the **Open IT Policy Library by Sorted Solution**. If you fork, copy, or incorporate these policies into your employee handbook:

- Please retain the attribution header.
- You are free to modify the policies to fit your organization.
- Attribution is appreciated but not legally required beyond the terms of the license below.

## License

This work is licensed under the [Creative Commons Attribution 4.0 International License (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/).

You are free to:

- **Share** — copy and redistribute the material in any medium or format
- **Adapt** — remix, transform, and build upon the material for any purpose, including commercial use

## Legal Disclaimer

These policy templates are provided as-is for informational and operational purposes. They do not constitute legal advice and do not replace consultation with qualified legal counsel. Sorted Solution is not liable for any damages or regulatory consequences arising from the use, modification, or implementation of these documents. AI vendor terms, features, and data handling practices change frequently — verify that all vendor-specific information is current before relying on it.
