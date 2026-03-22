# AI Acceptable Use Policy
**Open IT Policy Library by Sorted Solution** | [sortedsolution.com](https://www.sortedsolution.com/oitpl)<br>
*Version 1.0 — March 2026*
*Free to use, fork, and adapt at [github.com/sortedsol/Open-IT-Policy-Library](https://github.com/sortedsol/Open-IT-Policy-Library)* | [Download DOCX version](https://github.com/sortedsol/Open-IT-Policy-Library/raw/main/policies/general/AI-Acceptable-Use-Policy.docx)

---

## 1. Scope

This policy applies to everyone who does work for the company — employees, contractors, consultants, and interns. It applies regardless of what device you're using, where you're working, or whether the company provided the AI tool.

"AI tools" includes:

- Standalone AI assistants (ChatGPT, Claude, Gemini, Perplexity, etc.)
- AI features built into approved software (Microsoft 365 Copilot, Adobe Firefly, GitHub Copilot, Google Workspace Gemini features)
- Image generation tools (Midjourney, DALL·E, Stable Diffusion)
- AI-powered transcription, summarization, and meeting tools
- AI-powered note-taking and meeting bots (Otter, Fireflies, Granola, etc.)
- Browser-based summarizers, PDF viewers with built-in AI chat, and third-party plugins that send data to outside AI services
- Any browser extension, plugin, or add-on that sends data through an AI model — many of these tools quietly capture data in the background without you realizing it

---

## 2. Client and Contract Requirements Override This Policy

If a client contract, NDA, or regulatory requirement is stricter than this policy, the stricter rule wins. If a client agreement says "no AI," that means no AI — even if this policy would otherwise allow it. When in doubt, check with your manager before using AI tools on that client's data.

---

## 3. Key Concept: Zero-Data-Retention (ZDR)

When you type something into an AI tool or upload a file, what happens to that data? That's the key question. A **Zero-Data-Retention (ZDR) agreement** is a written promise from the AI vendor that:

1. Your inputs (prompts, uploaded files, pasted text) are **not stored** after processing
2. Your data is **not used to train** the vendor's AI models
3. This promise is in a **signed agreement**, not just a marketing page or FAQ

ZDR is one of the biggest factors in whether a tool is safe to use with company or client data. The company also looks at things like where the data is stored, what admin controls are available, and what our clients require of us. The bottom line: if the tool doesn't have written protections under your company's subscription, don't use it with any client, project, or confidential company data.

---

## 4. AI Tool Classification

### Tier 1 — Pre-Approved (IT-managed, enterprise protections confirmed)

These tools have been reviewed, set up, and approved by IT. You can use them with client and project data, following the Data Classification rules in Section 6.

| Tool | Condition | Notes |
|------|-----------|-------|
| Microsoft 365 Copilot / Copilot Chat | Must be licensed and turned on by the company under an eligible Microsoft 365 subscription | Copilot is an add-on — it's not included in M365 by default. Make sure you have the version with enterprise data protection (Copilot and Copilot Chat are different products with different licensing). See [Microsoft's DPA](https://www.microsoft.com/licensing/docs/view/Microsoft-Products-and-Services-Data-Protection-Addendum-DPA) and [Copilot privacy & data protection](https://learn.microsoft.com/en-us/copilot/microsoft-365/microsoft-365-copilot-privacy). |
| Adobe Firefly | Included in the company's Creative Cloud enterprise subscription | Adobe does not use enterprise content to train Firefly. See [Firefly Enterprise security fact sheet](https://www.adobe.com/content/dam/cc/en/trust-center/ungated/whitepapers/creative-cloud/adobe-firefly-fact-sheet.pdf) and [Adobe DPA](https://www.adobe.com/legal/terms/enterprise-licensing/data-protection.html). |
| GitHub Copilot Business/Enterprise | Company-managed subscription | Your prompts and suggestions are not used for training under Business/Enterprise plans (though some operational logging may still happen). See [GitHub Copilot data handling](https://resources.github.com/learn/pathways/copilot/essentials/how-github-copilot-handles-data/) and [product terms](https://docs.github.com/en/site-policy/github-terms/github-terms-for-additional-products-and-features). |
| Google Workspace Gemini | Accessed through the company's managed Google Workspace Business/Enterprise plan | Enterprise protections only apply through a managed Workspace account. See [Gemini for Workspace data protection](https://workspace.google.com/terms/gemini-for-google-workspace-data-protection.html) and [Google Workspace DPA](https://workspace.google.com/terms/dpa_terms.html). |

!!! tip "Company administrators"
    Update this table to match your actual subscriptions. A tool is only Tier 1 if your company has the specific license that includes enterprise data protections and IT has set it up and approved it.


### Tier 2 — Approved with Restrictions (enterprise protections confirmed, requires IT setup)

These tools offer data protections under certain subscription tiers but aren't part of the company's core software. They can be used with client and project data, but only after IT has confirmed the account is set up correctly.

| Tool | Required Tier | Key Restriction |
|------|--------------|-----------------|
| ChatGPT Business / Enterprise | Company-managed only | Your data is not used for training by default. Must be set up and managed by the company — personal subscriptions don't count. |
| OpenAI API | Set up by IT with approved settings | Zero-data-retention may only apply under certain configurations. IT must verify the settings before you use it with client data. |
| Claude for Work / Team / Enterprise | Company-managed only | The business plans handle data differently than the consumer product. Must be reviewed and approved by IT before use with client data. |
| Gemini for Google Workspace (non-managed) | Set up by IT | Enterprise protections only apply through a managed Workspace account. Consumer Gemini is not approved for confidential or client data. |

### Tier 3 — Approved for General Knowledge Only (No ZDR or unverified)

These tools can only be used for general questions that contain **zero** client data, project data, company financials, or internal business information. Think of them the same way you'd think of a Google search — don't type anything you wouldn't want to be public.

Examples: ChatGPT Free/Plus/Pro (consumer plans), Claude Free/Pro/Max (consumer plans), consumer Gemini, Perplexity Free, Midjourney (default plans), or any AI tool not listed in Tier 1 or Tier 2. Consumer plans may use your input to improve their AI models unless you've turned that off — but even with training disabled, these plans don't have the written protections the company needs for client or business data.

### Tier 4 — Prohibited

- Any AI tool that has been explicitly prohibited by IT
- Any AI browser extension not reviewed by IT (these often capture all text on every page you visit)
- AI tools that require uploading files to unknown or unvetted third-party servers
- "Jailbroken" or unofficial AI model wrappers

> **If a tool isn't listed in Tier 1 or Tier 2, it's Tier 3 by default.** You don't need to ask permission to use a Tier 3 tool for general knowledge questions. If you want a tool evaluated for Tier 1 or Tier 2, submit a request to IT.

---

## 5. Local Processing vs. Cloud-Routed AI

Not all AI tools send your data to someone else's server. Understanding the difference matters:

- **Local / on-device AI** runs entirely on your computer or the company's server. Your data never leaves the device. Examples: locally installed LLMs (Ollama, LM Studio), on-device transcription (Whisper running locally), and some features in desktop software that process data right on your workstation. This is the lowest risk for data exposure — but the output still needs the same professional review as anything else.

- **Cloud-routed AI** sends your input to the vendor's servers and sends a result back. This includes ChatGPT, Claude, Gemini, Midjourney, and most AI features in online software. This is where ZDR matters — without it, your data could be stored, logged, or used for training on the vendor's servers.

- **Hybrid tools** do some work locally and send other tasks to the cloud. Microsoft Copilot in M365, for example, works within your company's environment but still talks to Microsoft's AI servers. Adobe Firefly generates images on Adobe's servers. A good question to ask yourself: *where does my data go when I press Enter?*

If the company runs its own local AI models, those aren't automatically Tier 1 — IT still needs to evaluate them. But local processing does eliminate the risk of your data ending up on someone else's servers, which is what most of this policy is about.

---

## 6. Data Classification for AI Use

Not all data carries the same risk. This classification tells you what kind of data you can use with which AI tools.

### Level 1 — Public / General Knowledge

Information that's already public or has no confidentiality attached to it.

Examples: publicly available industry information, general regulatory questions, published research, publicly posted company marketing materials, general "how do I do this?" questions

**Permitted AI tiers:** 1, 2, 3

### Level 2 — Internal / Low Sensitivity

Company information that isn't public but wouldn't cause real harm if it got out.

Examples: internal meeting agendas (non-client), company process documentation, general templates, training materials, draft marketing content, non-confidential proposal boilerplate

**Permitted AI tiers:** 1, 2

### Level 3 — Confidential / Client Data

Client information, project work, and business data that the company is professionally or contractually obligated to protect.

Examples: client project files, work product and deliverables, client correspondence, client budgets and pricing, proposals with client-specific terms, internal financial data, vendor contracts, employee compensation data, strategic plans

**Permitted AI tiers:** 1 only

### Level 4 — Restricted

The most sensitive data — protected by specific legal requirements, strict NDAs, or regulations.

Examples: NDA-protected work (e.g., pre-announcement projects), security-sensitive materials, personally identifiable information (PII) of clients or their customers, protected health information (PHI), legal correspondence related to disputes or litigation, sealed or confidential bid documents, data subject to regulatory compliance requirements (HIPAA, SOX, GLBA, etc.)

**Permitted AI tiers:** 1 only, and only with explicit executive approval each time. Some Level 4 data may not be allowed in any AI tool at all, depending on the specific NDA or regulation.

---

## 7. Rules for AI Use

### 7.1 — Professional Review of AI-Generated Output

AI can produce output that looks right but is wrong, incomplete, or misleading. You're responsible for anything you put your name on, no matter how it was produced.

**The baseline rule:** If AI-generated output is going into a client deliverable, informing a business decision, or being shared outside the company, a qualified person must review it first.

!!! tip "Company administrators"
    Define your review requirements based on your industry and risk tolerance. At a minimum, consider this framework:

    - **Internal and informal use** (brainstorming, internal memos, research summaries): Check for factual accuracy before relying on the output.
    - **Client-facing deliverables** (reports, presentations, proposals): Have a manager or senior team member review before delivery.
    - **Technical or compliance-sensitive work** (financial analysis, regulatory filings, legal-adjacent content): Have a qualified subject matter expert review before it goes out.
    - **Documents requiring signatures or certifications:** The responsible party must independently verify any AI-assisted content.


### 7.2 — Disclosure and Transparency

- Be upfront with your team when AI played a big role in producing deliverables.
- If a client contract or RFP requires you to disclose AI use, do it.
- Don't pass off AI-generated content as original human work in situations where the distinction matters (proposals, qualifications, published articles).

### 7.3 — Intellectual Property and Copyright

- AI-generated images and text may not qualify for copyright protection. Don't rely on AI output as the sole basis for anything you plan to copyright or defend as intellectual property.
- Don't upload other people's copyrighted work into AI tools — that includes proprietary documents, copyrighted reference materials, and published content with restricted distribution.
- Before using AI-generated images in client deliverables or marketing, make sure the tool's terms of service actually give you commercial use rights under your subscription.

### 7.4 — AI for Code and Technical Work

If your team uses AI code assistants like GitHub Copilot, you must review and test any generated code before using it in production. Don't run AI-generated scripts in live systems without testing them in an isolated environment first and getting approval from a technical lead or manager.

### 7.5 — Data Minimization

Even when using a Tier 1 or Tier 2 tool, share as little data as possible. Before you type a prompt or upload a file, take a moment to remove client names, project names, dollar amounts, and personal contact info where you can. The less you share, the less there is to worry about if something goes wrong.

### 7.6 — Records Retention and Discoverability

Your AI conversations could become business records — especially if they influence decisions, inform deliverables, or contain information relevant to client work. Don't assume AI chats are casual and private. If AI output contributed to a business decision, save that output in the company's records system. Don't leave it sitting in a third-party chat history as the only copy.

### 7.7 — Output Storage

If AI output contains client or company information, copy it into the company's approved systems (project folders, document management, approved cloud storage). Don't leave it sitting in a third-party AI chat indefinitely. Once you've saved the relevant output to company systems, delete the AI conversation from the third-party platform.

### 7.8 — AI in Client Communications

Don't use AI to draft client communications in a way that misrepresents who actually wrote them. If you use AI to help draft a client email, you're still responsible for what it says, how it sounds, and whether it's accurate — same as if you'd used any other tool to help you write.

---

## 8. Prohibited Uses

No matter what tool or data type is involved, the following are never allowed:

1. Uploading large volumes of client files, complete project databases, or entire document libraries to any AI tool without written approval from management and confirmation that the tool is approved for that type of data
2. Using AI to generate signatures, certifications, or attestations
3. Using AI to produce financial calculations, tax filings, or regulatory submissions without a qualified professional independently verifying the results
4. Using AI to draft legal documents, contracts, or insurance claims without legal counsel reviewing them
5. Using AI as the main basis for employee performance reviews, HR decisions, or hiring/firing — AI can help with drafting, but final decisions must comply with employment law and company HR policy
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

!!! tip "Company administrators"
    Insert your actual IT contact method above.


---

## 10. New Tool Requests and Evaluation

Want to use a new AI tool for client or project work? Here's how to get it evaluated:

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
- **An executive or department head** must approve Level 4 data use, client-specific exceptions, and any AI use that goes beyond what this policy covers.

If you're not sure whether your situation needs more than IT approval, ask your manager.

---

## 12. Training

!!! tip "Company administrators"
    Consider requiring a short training session on this policy and your approved AI tools before giving staff access to Tier 1 or Tier 2 tools. An annual re-acknowledgment of this policy is a good idea. Training doesn't need to be complicated — a 30-minute walkthrough of the data levels, tool tiers, and what to do if something goes wrong is enough for most staff.


---

## 13. Enforcement

- IT may check AI tool usage through device management, browser history (on company devices), network logs, and software inventory.
- Violations will be handled through the company's standard disciplinary process.
- Repeated or intentional violations — especially ones that expose client data — may result in termination and will be reported to the company's liability insurance carrier if required.
- This policy will be reviewed and updated quarterly, or sooner if something significant changes with AI tools, vendor terms, or regulations.

---

## 14. Disclaimer

This policy covers the company's internal use of AI tools. It doesn't replace client-specific contract requirements, legal advice, or professional licensing obligations. AI vendor terms and features change frequently — the company is responsible for keeping this policy up to date.

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

*This policy is part of the [Open IT Policy Library](https://github.com/sortedsol/Open-IT-Policy-Library) by [Sorted Solution](https://www.sortedsolution.com). Free to use, fork, and adapt. Attribution appreciated.*
