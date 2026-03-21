# AI Acceptable Use Policy for AEC Firms
**Open IT Policy Library for AEC by Sorted Solution** | [sortedsolution.com](https://www.sortedsolution.com/oitpl)

*Version 1.0 — March 2026 | Free to use*

---

## Scope

This policy applies to all employees, contractors, subconsultants, and interns who use AI tools in connection with firm work — whether on firm-owned devices or personal devices, whether in the office or in the field, and whether the tool is provided by the firm or accessed independently.

"AI tools" includes:

- Standalone AI assistants (ChatGPT, Claude, Gemini, Perplexity, etc.)
- AI features built into approved software (Microsoft 365 Copilot, Adobe Firefly, ArchiCAD AI Assistant, Revit AI features, AutoCAD AI features, Bluebeam AI features, GitHub Copilot)
- Image generation tools (Midjourney, DALL·E, Stable Diffusion)
- AI-powered transcription, summarization, and meeting tools
- AI-powered note-taking and meeting bots (Otter, Fireflies, Granola, etc.)
- Browser-based summarizers, PDF viewers with embedded AI chat, and CAD/BIM plugins that route data through third-party AI services
- Any browser extension, plugin, or integration that routes data through an AI model — many of these tools capture data in the background without obvious prompts

---

## Client and Contract Requirements Override This Policy

Client-specific contract terms, NDAs, owner requirements, government requirements, and insurer requirements that are more restrictive than this policy take precedence. If a project contract prohibits the use of AI tools entirely, or restricts them beyond what this policy allows, the stricter rule applies. When in doubt, check with your project lead before using AI tools on that project's data.

---

## Key Concept: Zero-Data-Retention (ZDR)

A primary factor in evaluating whether an AI tool is acceptable for use with firm or project data is whether it offers a **Zero-Data-Retention (ZDR) agreement** — a contractual commitment from the AI vendor that:

1. Your inputs (prompts, uploaded files, pasted text) are **not stored** after processing
2. Your data is **not used to train** the vendor's AI models
3. The vendor provides this commitment in a **written data processing agreement**, not just a marketing FAQ

The firm also considers contractual data protections, data residency, admin controls, retention settings, security posture, and applicable client obligations when evaluating AI tools. For tools handling confidential or project data, written business or enterprise data protections are generally required. If a tool does not offer these protections under your firm's subscription tier, it must not be used with any client data, project data, or confidential firm information.

---

## AI Tool Classification

### Tier 1 — Pre-Approved (IT-managed, enterprise protections confirmed)

These tools have been evaluated by IT, are specifically licensed, configured, and approved by the firm, and may be used with project data subject to the Data Classification rules below.

| Tool | Condition | Notes |
|------|-----------|-------|
| Microsoft 365 Copilot / Copilot Chat | Must be licensed and enabled by the firm under an eligible Microsoft 365 subscription | Copilot is an add-on to eligible M365 plans, not included by default. Verify whether the user has Microsoft 365 Copilot or Copilot Chat with enterprise data protection — these offer different capabilities and licensing. Customer data is governed by the tenant's security and compliance controls. See [Microsoft's DPA](https://www.microsoft.com/licensing/docs/view/Microsoft-Products-and-Services-Data-Protection-Addendum-DPA) and [Copilot privacy & data protection](https://learn.microsoft.com/en-us/copilot/microsoft-365/microsoft-365-copilot-privacy). |
| Adobe Firefly | Included in firm's Creative Cloud enterprise subscription | Adobe does not train foundational Firefly models on enterprise content. See [Firefly Enterprise security fact sheet](https://www.adobe.com/content/dam/cc/en/trust-center/ungated/whitepapers/creative-cloud/adobe-firefly-fact-sheet.pdf) and [Adobe DPA](https://www.adobe.com/legal/terms/enterprise-licensing/data-protection.html). |
| GitHub Copilot Business/Enterprise | Firm-managed subscription | Prompts and suggestions are not used for model training under Business/Enterprise terms; operational logging and retention may still apply. See [GitHub Copilot data handling](https://resources.github.com/learn/pathways/copilot/essentials/how-github-copilot-handles-data/) and [product terms](https://docs.github.com/en/site-policy/github-terms/github-terms-for-additional-products-and-features). |
| ArchiCAD AI Assistant / AI Visualizer | Part of licensed ArchiCAD Collaborate or Studio plan | Graphisoft does not use project data for AI training. See [AI Assistant details](https://www.graphisoft.com/en-us/plans-and-products/ai-assistant/) and [Graphisoft legal/DPA](https://www.graphisoft.com/en-us/company/legal). |
| Revit AI features (Generative Design, AI Assistant) | Part of licensed Revit / AEC Collection subscription | Covered under [Autodesk's DPA](https://damassets.autodesk.net/content/dam/autodesk/www/pdfs/Autodesk_DPA_Online.pdf). See [Revit AI features overview](https://www.autodesk.com/support/technical/article/caas/sfdcarticles/sfdcarticles/What-AI-features-are-available-in-Revit.html) and [Autodesk Trust Center](https://www.autodesk.com/trust/privacy). |
| AutoCAD AI features (Smart Blocks, Autodesk Assistant) | Part of licensed AutoCAD subscription | Covered under [Autodesk's DPA](https://damassets.autodesk.net/content/dam/autodesk/www/pdfs/Autodesk_DPA_Online.pdf). See [AutoCAD AI features overview](https://www.autodesk.com/support/technical/article/caas/sfdcarticles/sfdcarticles/What-are-the-AutoCAD-AI-driven-features.html). |
| Bluebeam AI features (AI-Review, AI-Match) | Part of licensed Bluebeam Revu or Bluebeam Max subscription | See [Bluebeam AI & Innovation](https://www.bluebeam.com/product/ai-and-innovation/) and [Bluebeam DPA](https://www.bluebeam.com/legal/data-processing-addendum/). |

> **Firm administrators:** Update this table to reflect your actual subscriptions and configurations. A tool listed here is only Tier 1 if your firm holds the specific license tier that includes enterprise data protections and has been configured and approved by IT for the relevant data types and workflows.

### Tier 2 — Approved with Restrictions (enterprise protections confirmed, requires IT setup)

These tools offer ZDR under specific subscription tiers but are not part of the firm's core software stack. They may be used with project data only after IT has confirmed the firm's account is configured correctly.

| Tool | Required Tier | Key Restriction |
|------|--------------|-----------------|
| ChatGPT Business / Enterprise | Firm-managed only | Business data is not used for training by default. Must be provisioned and managed by the firm — personal subscriptions do not qualify. |
| OpenAI API | Provisioned by IT under approved retention settings | Zero-data-retention may be available only for qualifying configurations. IT must verify retention settings before use with project data. |
| Claude for Work / Team / Enterprise | Firm-managed only | Commercial terms govern data handling separately from consumer products. Must be reviewed and approved by IT before use with project data. |
| Gemini for Google Workspace | Accessed through firm's managed Google Workspace environment | Enterprise protections apply when Gemini is accessed through a managed Workspace account. Consumer Gemini remains non-approved for confidential or project data. |

### Tier 3 — Approved for General Knowledge Only (No ZDR or unverified)

These tools may be used only for general-purpose questions that contain **zero** client data, project data, firm financials, or internal business information. Treat them the way you would treat a public Google search.

Examples: ChatGPT Free/Plus/Pro (consumer plans), Claude Free/Pro/Max (consumer plans), consumer Gemini, Perplexity Free, Midjourney (default plans), any AI tool not listed in Tier 1 or Tier 2. Consumer plans may use content for model improvement unless the user has explicitly disabled training — but even with training disabled, these plans lack the contractual protections required for firm data.

### Tier 4 — Prohibited

- Any AI tool that has been explicitly prohibited by IT
- Any AI browser extension not reviewed by IT (these often capture all text on every page you visit)
- AI tools that require uploading files to unknown or unvetted third-party servers
- "Jailbroken" or unofficial AI model wrappers

> **If a tool is not listed in Tier 1 or Tier 2, it is Tier 3 by default.** Staff do not need to submit a request to use a Tier 3 tool for general knowledge queries. Staff must submit a request to IT if they want a tool evaluated for Tier 1 or Tier 2 classification.

---

## Local Processing vs. Cloud-Routed AI

Not all AI tools send your data to a remote server. Understanding the difference matters for risk assessment:

- **Local / on-device AI** runs the model entirely on your computer or your firm's server. Your data never leaves the device. Examples: locally installed LLMs (Ollama, LM Studio), on-device transcription (Whisper running locally), and certain desktop features in tools like ArchiCAD, Revit, AutoCAD, or Bluebeam that process data on your workstation without a cloud connection. Local processing carries the lowest data exposure risk because there is no network transmission — but the output still requires the same professional review.

- **Cloud-routed AI** sends your input to the vendor's servers for processing and returns a result. This includes ChatGPT, Claude, Gemini, Midjourney, and most AI features in SaaS products. Cloud routing is where ZDR status matters — without it, your data may be stored, logged, or used for training on the vendor's infrastructure.

- **Hybrid tools** may process some operations locally and route others to the cloud. Microsoft Copilot in M365, for example, processes within your tenant environment but still communicates with Microsoft's AI infrastructure. Adobe Firefly generates images server-side. When evaluating a tool, ask: *where does the data go when I press Enter?*

If the firm deploys local AI models for internal use, those tools are not automatically Tier 1 — IT must still evaluate them for security, licensing, and output quality. But local processing does eliminate the third-party data exposure risk that drives most of this policy.

---

## Data Classification for AI Use

Not all firm data carries the same risk. The following classification determines what may be shared with AI tools at each tier.

### Level 1 — Public / General Knowledge

Information that is already publicly available or carries no confidentiality obligation.

*AEC examples:* general building code questions, publicly available zoning regulations, material specification lookups, general construction methodology questions, publicly posted project photos (post-completion, with client permission)

**Permitted AI tiers:** 1, 2, 3

### Level 2 — Internal / Low Sensitivity

Firm information that is not public but would cause minimal harm if disclosed.

*AEC examples:* internal meeting agendas (non-client), firm process documentation, general templates, training materials, draft marketing content, non-confidential RFP response boilerplate

**Permitted AI tiers:** 1, 2

### Level 3 — Confidential / Project Data

Client project information, design work, and business data protected by professional obligation or contract.

*AEC examples:* concept sketches and design development drawings, construction documents (pre-bid and post-bid), BIM models and associated data, project specifications, client correspondence, client budgets and fee proposals, site photography and survey data, structural and MEP engineering calculations, energy models, subcontractor pricing, project schedules with cost data

**Permitted AI tiers:** 1 only

### Level 4 — Restricted

Information subject to specific legal protections, NDAs with heightened terms, or regulatory requirements.

*AEC examples:* NDA-protected design work (e.g., pre-announcement projects for public clients), security-sensitive facility designs (government, healthcare, data centers), critical infrastructure projects (utilities, transportation, water treatment), export-controlled work, defense or law enforcement facility designs, personally identifiable information (PII) of building occupants, legal correspondence related to claims or disputes, sealed bid documents, HIPAA-adjacent healthcare facility programming data

**Permitted AI tiers:** 1 only, and only with explicit principal/partner approval per instance. Some Level 4 data may be excluded from AI use entirely based on the specific NDA or regulatory requirement.

---

## Rules for AI Use in AEC Work

### 6.1 — Professional Review of AI-Generated Output

AI tools can produce plausible-looking output that is incorrect, incomplete, or unsuitable for the project context. This is especially consequential in AEC work, where errors can affect life safety, code compliance, and professional liability.

**The baseline rule:** Every AI-generated output that will appear in a client deliverable, be used in a design decision, or inform engineering calculations must be reviewed by a qualified professional before use.

You are responsible for anything you present as your own work, regardless of how it was produced. AI-generated content in stamped or sealed documents must never be the sole basis for any element — the professional of record is responsible for independent verification.

> **Firms:** Define your review requirements based on your practice areas, risk tolerance, and licensure obligations. At a minimum, consider the following framework and customize it to match your professional liability insurance requirements. Some carriers are issuing specific guidance on AI-generated work product — check with your broker.
>
> - **Conceptual and internal use** (brainstorming, internal memos, research summaries): Review for factual accuracy before relying on the output.
> - **Client-facing deliverables** (reports, presentations, renderings shown to clients): Review by a project manager or senior staff member before delivery.
> - **Technical and code-compliance work** (calculations, code analysis, specification language, drawing annotations): Review by a licensed professional appropriate to the discipline before incorporation into documents of record.
> - **Stamped or sealed documents:** Independent verification by the professional of record required before any AI-assisted content is incorporated.

### 6.2 — Disclosure and Transparency

- Be transparent with your team when AI tools played a significant role in producing deliverables.
- If a client contract or RFP requires disclosure of AI use, comply fully.
- Do not represent AI-generated content as original human work in contexts where the distinction matters (proposals, qualifications, published articles).

### 6.3 — Intellectual Property and Copyright

- AI-generated images and text may not be eligible for copyright protection. Do not rely on AI-generated content as the sole basis for work you intend to register or defend as intellectual property.
- Do not upload copyrighted third-party materials (other firms' drawings, copyrighted reference images, published standards with restricted distribution) into AI tools.
- Before using AI-generated images in client deliverables or marketing, confirm that the tool's terms of service grant you commercial use rights under your subscription tier.

### 6.4 — AI for Code and Computational Design

If your firm uses computational design tools (Grasshopper, Dynamo, custom scripts), AI code assistants like GitHub Copilot can be productive — but generated code must be reviewed and tested before use in production workflows. Do not deploy AI-generated scripts that modify BIM models or automate drawing production without testing in an isolated environment first and getting approval from a firm principal or partner.

### 6.5 — Data Minimization

Even when using a Tier 1 or Tier 2 tool, minimize the data you share. Before submitting a prompt or uploading a file, strip out client names, project names, site addresses, fee amounts, personal contact information, and other identifying details where feasible. The less specific data you share with any AI tool, the lower the risk if something goes wrong.

### 6.6 — Records Retention and Discoverability

AI prompts and outputs may become business records — particularly if they influence design decisions, inform engineering calculations, or contribute to client deliverables. Do not assume that AI conversations are informal or undiscoverable. If AI-generated content contributes to a project decision, the relevant output should be saved in the firm's approved project records system, not left only in a third-party chat history.

### 6.7 — Output Storage

AI-generated output containing project or firm information must be copied into approved firm systems (project folders, document management, approved cloud storage) and not left indefinitely in third-party AI chat histories. Delete AI conversations containing project data from third-party platforms once the relevant output has been captured in firm systems.

### 6.8 — AI in Client Communications

Do not use AI tools to draft client communications that misrepresent the level of human involvement. If AI is used to help draft a client email, the sender is responsible for its content, tone, and accuracy — the same as any other tool used to assist in writing.

---

## Prohibited Uses

Regardless of tool tier or data classification, the following uses of AI are prohibited:

1. Uploading complete construction document sets, full BIM models, or full project specifications to any AI tool without documented project lead approval and confirmation that the tool is specifically approved for that dataset type — the volume of data increases exposure risk
2. Using AI to generate professional stamps, seals, or signatures
3. Using AI to produce structural, mechanical, electrical, or plumbing calculations that will be used without independent verification by a licensed engineer
4. Using AI to draft legal documents, contracts, or insurance claims without legal counsel review
5. Using AI as the sole or primary basis for employee performance reviews, HR decisions, or hiring/firing recommendations — AI may be used to assist with drafting, but final decisions and content must comply with employment law and firm HR policy
6. Circumventing tool restrictions (e.g., using a personal ChatGPT Free account to do work that requires a Tier 1 or Tier 2 tool because "it's faster")
7. Installing AI browser extensions or plugins without IT approval
8. Using AI tools to reverse-engineer, replicate, or analyze competitors' proprietary work

---

## Incident Response: Accidental Data Exposure

If you accidentally upload confidential or restricted data to an AI tool that does not have ZDR protections:

1. **Stop immediately.** Do not continue the conversation or upload additional data.
2. **Screenshot or copy the conversation** before closing it — this preserves evidence of what was shared.
3. **Delete the conversation** from the AI tool if the platform allows it (ChatGPT: delete from sidebar; Claude: delete conversation; Gemini: delete activity).
4. **Notify IT within 1 business hour** at [INSERT IT CONTACT: email/Slack/phone]. Include: which tool, what data was shared, which client/project, and whether you were able to delete the conversation.
5. **IT will assess** whether the client needs to be notified based on the firm's contractual obligations and the sensitivity of the data involved.
6. **Do not attempt to handle this quietly.** Fast reporting is not punished — delayed reporting creates legal exposure.

> **Firms:** Insert your actual IT contact method above.

---

## New Tool Requests and Evaluation

To request a new AI tool be evaluated for Tier 1 or Tier 2 classification:

1. Submit a request to IT with: tool name, vendor, intended use case, subscription tier being considered, and a link to the vendor's data processing terms.
2. IT will evaluate the tool against the firm's data protection criteria, including ZDR status, contractual protections, admin controls, and data residency.
3. IT will respond with an approval, denial, or request for more information.
4. Approved tools will be added to the classification table in this policy and communicated to all staff.

Do not use a tool at Tier 1 or Tier 2 classification levels until IT has confirmed the evaluation.

---

## Approval Authority

Different types of AI-related decisions require different levels of approval:

- **IT** reviews and approves the technical and security fit of AI tools (tool classification, configuration, account provisioning).
- **Legal or operations** reviews contract and data processing terms when needed, particularly for tools handling Level 3 or Level 4 data.
- **A firm principal or project executive** approves Level 4 data use, project-specific exceptions, and any AI use that falls outside the standard rules in this policy.

If you are unsure whether your intended use requires approval beyond IT, ask your project lead.

---

## Training

> **Firms:** Consider requiring short training on this policy and on the specific AI tools your firm has approved before granting staff access to Tier 1 or Tier 2 tools. Annual re-acknowledgment of this policy is recommended. Training does not need to be elaborate — a 30-minute walkthrough of the data classification levels, tool tiers, and incident reporting steps is sufficient for most staff.

---

## Enforcement

- IT may audit AI tool usage through endpoint management, browser history (on firm-managed devices), network traffic logs, and software inventory.
- Violations of this policy will be addressed through the firm's standard disciplinary process.
- Repeated or intentional violations — particularly those involving client data exposure — may result in termination and will be reported to the firm's professional liability carrier if required by policy terms.
- This policy will be reviewed and updated quarterly, or sooner if a significant change occurs in AI tool capabilities, vendor terms, or regulatory requirements.

---

## Disclaimer

This policy governs internal firm use of AI tools and does not replace project-specific contractual requirements, legal advice, or professional licensure obligations. AI vendor terms, features, and data handling practices change frequently — the firm is responsible for verifying that the information in this policy remains current.

---

## Acknowledgment

I have read and understand this AI Acceptable Use Policy. I understand that violations may result in disciplinary action and that I am responsible for the appropriate use of AI tools in my work.

**Name:** _______________________________________________

**Signature:** _______________________________________________

**Date:** _______________________________________________

---

## Revision History

| Version | Date | Summary |
|---------|------|---------|
| 1.0 | March 2026 | Initial release |

---

*This policy is part of the [Open IT Policy Library for AEC](https://github.com/sortedsol/Open-IT-Policy-Library) by [Sorted Solution](https://sortedsolution.com). Free to use, fork, and adapt. Attribution appreciated.*
