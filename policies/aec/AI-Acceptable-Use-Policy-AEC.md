# AI Acceptable Use Policy for AEC Firms
**Open IT Policy Library for AEC by Sorted Solution** | [sortedsolution.com](https://www.sortedsolution.com/oitpl)<br>
*Version 1.0 — March 2026*
*Free to use* | [Download DOCX version](AI-Acceptable-Use-Policy-AEC.docx)

---

## 1. Scope

This policy applies to everyone who does work for the firm — employees, contractors, subconsultants, and interns. It applies regardless of what device you're using, where you're working, or whether the firm provided the AI tool.

"AI tools" includes:

- Standalone AI assistants (ChatGPT, Claude, Gemini, Perplexity, etc.)
- AI features built into approved software (Microsoft 365 Copilot, Adobe Firefly, ArchiCAD AI Assistant, Revit AI features, AutoCAD AI features, Bluebeam AI features, GitHub Copilot)
- Image generation tools (Midjourney, DALL·E, Stable Diffusion)
- AI-powered transcription, summarization, and meeting tools
- AI-powered note-taking and meeting bots (Otter, Fireflies, Granola, etc.)
- Browser-based summarizers, PDF viewers with built-in AI chat, and CAD/BIM plugins that send data to outside AI services
- Any browser extension, plugin, or add-on that sends data through an AI model — many of these tools quietly capture data in the background without you realizing it

---

## 2. Client and Contract Requirements Override This Policy

If a client contract, NDA, or government requirement is stricter than this policy, the stricter rule wins. If a project contract says "no AI," that means no AI — even if this policy would otherwise allow it. When in doubt, check with your project lead before using AI tools on that project's data.

---

## 3. Key Concept: Zero-Data-Retention (ZDR)

When you type something into an AI tool or upload a file, what happens to that data? That's the key question. A **Zero-Data-Retention (ZDR) agreement** is a written promise from the AI vendor that:

1. Your inputs (prompts, uploaded files, pasted text) are **not stored** after processing
2. Your data is **not used to train** the vendor's AI models
3. This promise is in a **signed agreement**, not just a marketing page or FAQ

ZDR is one of the biggest factors in whether a tool is safe to use with firm or project data. The firm also looks at things like where the data is stored, what admin controls are available, and what our clients require of us. The bottom line: if the tool doesn't have written protections under your firm's subscription, don't use it with any client, project, or confidential firm data.

---

## 4. AI Tool Classification

### Tier 1 — Pre-Approved (IT-managed, enterprise protections confirmed)

These tools have been reviewed, set up, and approved by IT. You can use them with project data, following the Data Classification rules in Section 6.

| Tool | Condition | Notes |
|------|-----------|-------|
| Microsoft 365 Copilot / Copilot Chat | Must be licensed and turned on by the firm under an eligible Microsoft 365 subscription | Copilot is an add-on — it's not included in M365 by default. Make sure you have the version with enterprise data protection (Copilot and Copilot Chat are different products with different licensing). See [Microsoft's DPA](https://www.microsoft.com/licensing/docs/view/Microsoft-Products-and-Services-Data-Protection-Addendum-DPA) and [Copilot privacy & data protection](https://learn.microsoft.com/en-us/copilot/microsoft-365/microsoft-365-copilot-privacy). |
| Adobe Firefly | Included in the firm's Creative Cloud enterprise subscription | Adobe does not use enterprise content to train Firefly. See [Firefly Enterprise security fact sheet](https://www.adobe.com/content/dam/cc/en/trust-center/ungated/whitepapers/creative-cloud/adobe-firefly-fact-sheet.pdf) and [Adobe DPA](https://www.adobe.com/legal/terms/enterprise-licensing/data-protection.html). |
| GitHub Copilot Business/Enterprise | Firm-managed subscription | Your prompts and suggestions are not used for training under Business/Enterprise plans (though some operational logging may still happen). See [GitHub Copilot data handling](https://resources.github.com/learn/pathways/copilot/essentials/how-github-copilot-handles-data/) and [product terms](https://docs.github.com/en/site-policy/github-terms/github-terms-for-additional-products-and-features). |
| ArchiCAD AI Assistant / AI Visualizer | Part of a licensed ArchiCAD Collaborate or Studio plan | Graphisoft does not use your project data to train AI. See [AI Assistant details](https://www.graphisoft.com/en-us/plans-and-products/ai-assistant/) and [Graphisoft legal/DPA](https://www.graphisoft.com/en-us/company/legal). |
| Revit AI features (Generative Design, AI Assistant) | Part of a licensed Revit / AEC Collection subscription | Covered under [Autodesk's DPA](https://damassets.autodesk.net/content/dam/autodesk/www/pdfs/Autodesk_DPA_Online.pdf). See [Revit AI features overview](https://www.autodesk.com/support/technical/article/caas/sfdcarticles/sfdcarticles/What-AI-features-are-available-in-Revit.html) and [Autodesk Trust Center](https://www.autodesk.com/trust/privacy). |
| AutoCAD AI features (Smart Blocks, Autodesk Assistant) | Part of a licensed AutoCAD subscription | Covered under [Autodesk's DPA](https://damassets.autodesk.net/content/dam/autodesk/www/pdfs/Autodesk_DPA_Online.pdf). See [AutoCAD AI features overview](https://www.autodesk.com/support/technical/article/caas/sfdcarticles/sfdcarticles/What-are-the-AutoCAD-AI-driven-features.html). |
| Bluebeam AI features (AI-Review, AI-Match) | Part of a licensed Bluebeam Revu or Bluebeam Max subscription | See [Bluebeam AI & Innovation](https://www.bluebeam.com/product/ai-and-innovation/) and [Bluebeam DPA](https://www.bluebeam.com/legal/data-processing-addendum/). |

> **Firm administrators:** Update this table to match your actual subscriptions. A tool is only Tier 1 if your firm has the specific license that includes enterprise data protections and IT has set it up and approved it.

### Tier 2 — Approved with Restrictions (enterprise protections confirmed, requires IT setup)

These tools offer data protections under certain subscription tiers but aren't part of the firm's core software. They can be used with project data, but only after IT has confirmed the account is set up correctly.

| Tool | Required Tier | Key Restriction |
|------|--------------|-----------------|
| ChatGPT Business / Enterprise | Firm-managed only | Your data is not used for training by default. Must be set up and managed by the firm — personal subscriptions don't count. |
| OpenAI API | Set up by IT with approved settings | Zero-data-retention may only apply under certain configurations. IT must verify the settings before you use it with project data. |
| Claude for Work / Team / Enterprise | Firm-managed only | The business plans handle data differently than the consumer product. Must be reviewed and approved by IT before use with project data. |
| Gemini for Google Workspace | Accessed through the firm's managed Google Workspace | Enterprise protections only apply through a managed Workspace account. Consumer Gemini is not approved for confidential or project data. |

### Tier 3 — Approved for General Knowledge Only (No ZDR or unverified)

These tools can only be used for general questions that contain **zero** client data, project data, firm financials, or internal business information. Think of them the same way you'd think of a Google search — don't type anything you wouldn't want to be public.

Examples: ChatGPT Free/Plus/Pro (consumer plans), Claude Free/Pro/Max (consumer plans), consumer Gemini, Perplexity Free, Midjourney (default plans), or any AI tool not listed in Tier 1 or Tier 2. Consumer plans may use your input to improve their AI models unless you've turned that off — but even with training disabled, these plans don't have the written protections the firm needs for client or project data.

### Tier 4 — Prohibited

- Any AI tool that has been explicitly prohibited by IT
- Any AI browser extension not reviewed by IT (these often capture all text on every page you visit)
- AI tools that require uploading files to unknown or unvetted third-party servers
- "Jailbroken" or unofficial AI model wrappers

> **If a tool isn't listed in Tier 1 or Tier 2, it's Tier 3 by default.** You don't need to ask permission to use a Tier 3 tool for general knowledge questions. If you want a tool evaluated for Tier 1 or Tier 2, submit a request to IT.

---

## 5. Local Processing vs. Cloud-Routed AI

Not all AI tools send your data to someone else's server. Understanding the difference matters:

- **Local / on-device AI** runs entirely on your computer or the firm's server. Your data never leaves the device. Examples: locally installed LLMs (Ollama, LM Studio), on-device transcription (Whisper running locally), and some features in ArchiCAD, Revit, AutoCAD, or Bluebeam that process data right on your workstation. This is the lowest risk for data exposure — but the output still needs the same professional review as anything else.

- **Cloud-routed AI** sends your input to the vendor's servers and sends a result back. This includes ChatGPT, Claude, Gemini, Midjourney, and most AI features in online software. This is where ZDR matters — without it, your data could be stored, logged, or used for training on the vendor's servers.

- **Hybrid tools** do some work locally and send other tasks to the cloud. Microsoft Copilot in M365, for example, works within your firm's environment but still talks to Microsoft's AI servers. Adobe Firefly generates images on Adobe's servers. A good question to ask yourself: *where does my data go when I press Enter?*

If the firm runs its own local AI models, those aren't automatically Tier 1 — IT still needs to evaluate them. But local processing does eliminate the risk of your data ending up on someone else's servers, which is what most of this policy is about.

---

## 6. Data Classification for AI Use

Not all data carries the same risk. This classification tells you what kind of data you can use with which AI tools.

### Level 1 — Public / General Knowledge

Information that's already public or has no confidentiality attached to it.

*AEC examples:* general building code questions, publicly available zoning regulations, material specification lookups, general construction methodology questions, publicly posted project photos (post-completion, with client permission)

**Permitted AI tiers:** 1, 2, 3

### Level 2 — Internal / Low Sensitivity

Firm information that isn't public but wouldn't cause real harm if it got out.

*AEC examples:* internal meeting agendas (non-client), firm process documentation, general templates, training materials, draft marketing content, non-confidential RFP response boilerplate

**Permitted AI tiers:** 1, 2

### Level 3 — Confidential / Project Data

Client project information, design work, and business data that we're professionally or contractually obligated to protect.

*AEC examples:* concept sketches and design development drawings, construction documents (pre-bid and post-bid), BIM models and associated data, project specifications, client correspondence, client budgets and fee proposals, site photography and survey data, structural and MEP engineering calculations, energy models, subcontractor pricing, project schedules with cost data

**Permitted AI tiers:** 1 only

### Level 4 — Restricted

The most sensitive data — protected by specific legal requirements, strict NDAs, or regulations.

*AEC examples:* NDA-protected design work (e.g., pre-announcement projects for public clients), security-sensitive facility designs (government, healthcare, data centers), critical infrastructure projects (utilities, transportation, water treatment), export-controlled work, defense or law enforcement facility designs, personally identifiable information (PII) of building occupants, legal correspondence related to claims or disputes, sealed bid documents, HIPAA-adjacent healthcare facility programming data

**Permitted AI tiers:** 1 only, and only with explicit principal/partner approval each time. Some Level 4 data may not be allowed in any AI tool at all, depending on the specific NDA or regulation.

---

## 7. Rules for AI Use in AEC Work

### 7.1 — Professional Review of AI-Generated Output

AI can produce output that looks right but is wrong, incomplete, or doesn't fit the project. In AEC work, that's a serious problem — errors can affect life safety, code compliance, and professional liability.

**The baseline rule:** If AI-generated output is going into a client deliverable, informing a design decision, or feeding into engineering calculations, a qualified professional must review it first.

You are responsible for anything you put your name on, no matter how it was produced. AI-generated content in stamped or sealed documents must never stand on its own — the professional of record must independently verify it.

> **Firms:** Define your review requirements based on your practice areas and risk tolerance. Some insurance carriers are issuing specific guidance on AI-generated work product — check with your broker. At a minimum, consider this framework:
>
> - **Conceptual and internal use** (brainstorming, internal memos, research summaries): Check for factual accuracy before relying on the output.
> - **Client-facing deliverables** (reports, presentations, renderings shown to clients): Have a project manager or senior staff member review before delivery.
> - **Technical and code-compliance work** (calculations, code analysis, specification language, drawing annotations): Have a licensed professional in the appropriate discipline review before it goes into documents of record.
> - **Stamped or sealed documents:** The professional of record must independently verify any AI-assisted content before it's incorporated.

### 7.2 — Disclosure and Transparency

- Be upfront with your team when AI played a big role in producing deliverables.
- If a client contract or RFP requires you to disclose AI use, do it.
- Don't pass off AI-generated content as original human work in situations where the distinction matters (proposals, qualifications, published articles).

### 7.3 — Intellectual Property and Copyright

- AI-generated images and text may not qualify for copyright protection. Don't rely on AI output as the sole basis for anything you plan to copyright or defend as intellectual property.
- Don't upload other people's copyrighted work into AI tools — that includes other firms' drawings, copyrighted reference images, and published standards with restricted distribution.
- Before using AI-generated images in client deliverables or marketing, make sure the tool's terms of service actually give you commercial use rights under your subscription.

### 7.4 — AI for Code and Computational Design

If your firm uses computational design tools (Grasshopper, Dynamo, custom scripts), AI code assistants like GitHub Copilot can be helpful — but you must review and test any generated code before using it in real workflows. Don't run AI-generated scripts that modify BIM models or automate drawing production without testing them in an isolated environment first and getting approval from a firm principal or partner.

### 7.5 — Data Minimization

Even when using a Tier 1 or Tier 2 tool, share as little data as possible. Before you type a prompt or upload a file, take a moment to remove client names, project names, site addresses, fee amounts, and personal contact info where you can. The less you share, the less there is to worry about if something goes wrong.

### 7.6 — Records Retention and Discoverability

Your AI conversations could become business records — especially if they influence design decisions, feed into calculations, or end up in client deliverables. Don't assume AI chats are casual and private. If AI output contributed to a project decision, save that output in the firm's project records system. Don't leave it sitting in a third-party chat history as the only copy.

### 7.7 — Output Storage

If AI output contains project or firm information, copy it into the firm's approved systems (project folders, document management, approved cloud storage). Don't leave it sitting in a third-party AI chat indefinitely. Once you've saved the relevant output to firm systems, delete the AI conversation from the third-party platform.

### 7.8 — AI in Client Communications

Don't use AI to draft client communications in a way that misrepresents who actually wrote them. If you use AI to help draft a client email, you're still responsible for what it says, how it sounds, and whether it's accurate — same as if you'd used any other tool to help you write.

---

## 8. Prohibited Uses

No matter what tool or data type is involved, the following are never allowed:

1. Uploading full construction document sets, complete BIM models, or entire project specifications to any AI tool without written project lead approval and confirmation that the tool is approved for that type of data — the sheer volume increases the risk
2. Using AI to generate professional stamps, seals, or signatures
3. Using AI to produce structural, mechanical, electrical, or plumbing calculations without a licensed engineer independently verifying the results
4. Using AI to draft legal documents, contracts, or insurance claims without legal counsel reviewing them
5. Using AI as the main basis for employee performance reviews, HR decisions, or hiring/firing — AI can help with drafting, but final decisions must comply with employment law and firm HR policy
6. Working around tool restrictions (e.g., using a personal ChatGPT Free account to do work that needs a Tier 1 or Tier 2 tool because "it's faster")
7. Installing AI browser extensions or plugins without IT approval
8. Using AI to reverse-engineer, copy, or analyze competitors' proprietary work

---

## 9. Incident Response: Accidental Data Exposure

If you accidentally share confidential or restricted data with an AI tool that doesn't have ZDR protections:

1. **Stop immediately.** Don't continue the conversation or upload anything else.
2. **Screenshot or copy the conversation** before closing it — you need a record of what was shared.
3. **Delete the conversation** from the AI tool if you can (ChatGPT: delete from sidebar; Claude: delete conversation; Gemini: delete activity).
4. **Tell IT within 1 business hour** at [INSERT IT CONTACT: email/Slack/phone]. Include: which tool, what data was shared, which client/project, and whether you were able to delete the conversation.
5. **IT will determine next steps**, including whether the client needs to be notified.
6. **Don't try to handle this quietly.** Reporting quickly is not punished — waiting to report it creates legal risk.

> **Firms:** Insert your actual IT contact method above.

---

## 10. New Tool Requests and Evaluation

Want to use a new AI tool for project work? Here's how to get it evaluated:

1. Send IT a request with: the tool name, vendor, what you want to use it for, which subscription tier you're looking at, and a link to the vendor's data processing terms.
2. IT will review the tool's data protections, ZDR status, admin controls, and where data is stored.
3. IT will get back to you with an approval, denial, or follow-up questions.
4. Approved tools will be added to the classification table in this policy and announced to all staff.

Don't use a tool at Tier 1 or Tier 2 levels until IT has finished the evaluation.

---

## 11. Approval Authority

Different decisions need different levels of approval:

- **IT** decides whether a tool is technically safe and properly set up (tool classification, configuration, account setup).
- **Legal or operations** reviews contract and data terms when needed, especially for tools handling Level 3 or Level 4 data.
- **A firm principal or project executive** must approve Level 4 data use, project-specific exceptions, and any AI use that goes beyond what this policy covers.

If you're not sure whether your situation needs more than IT approval, ask your project lead.

---

## 12. Training

> **Firms:** Consider requiring a short training session on this policy and your approved AI tools before giving staff access to Tier 1 or Tier 2 tools. An annual re-acknowledgment of this policy is a good idea. Training doesn't need to be complicated — a 30-minute walkthrough of the data levels, tool tiers, and what to do if something goes wrong is enough for most staff.

---

## 13. Enforcement

- IT may check AI tool usage through device management, browser history (on firm devices), network logs, and software inventory.
- Violations will be handled through the firm's standard disciplinary process.
- Repeated or intentional violations — especially ones that expose client data — may result in termination and will be reported to the firm's liability insurance carrier if required.
- This policy will be reviewed and updated quarterly, or sooner if something significant changes with AI tools, vendor terms, or regulations.

---

## 14. Disclaimer

This policy covers the firm's internal use of AI tools. It doesn't replace project-specific contract requirements, legal advice, or your professional licensure obligations. AI vendor terms and features change frequently — the firm is responsible for keeping this policy up to date.

---

## 15. Acknowledgment

I have read and understand this AI Acceptable Use Policy. I understand that violations may result in disciplinary action and that I am responsible for using AI tools appropriately in my work.

**Name:** _______________________________________________

**Signature:** _______________________________________________

**Date:** _______________________________________________

---

## 16. Revision History

| Version | Date | Summary |
|---------|------|---------|
| 1.0 | March 2026 | Initial release |

---

*This policy is part of the [Open IT Policy Library for AEC](https://github.com/sortedsol/Open-IT-Policy-Library) by [Sorted Solution](https://sortedsolution.com). Free to use, fork, and adapt. Attribution appreciated.*
