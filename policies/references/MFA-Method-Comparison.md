# MFA Method Comparison & Phishing Resistance Matrix
**Open IT Policy Library by Sorted Solution** | [sortedsolution.com](https://www.sortedsolution.com/oitpl)<br>
*Last verified: March 2026*
*Free to use, fork, and adapt at [github.com/sortedsol/Open-IT-Policy-Library](https://github.com/sortedsol/Open-IT-Policy-Library)* | [Download DOCX version](https://github.com/sortedsol/Open-IT-Policy-Library/raw/main/policies/references/MFA-Method-Comparison.docx)

---

## 1. What This Is

This is a reference page that compares common multi-factor authentication (MFA) methods side by side — rated on phishing resistance, user friction, cost, and how practical they are for small and mid-sized businesses.

MFA is the single most effective thing a company can do to prevent account compromise. All three major authorities (NIST, Microsoft, and CIS) agree on that. But not all MFA methods offer the same level of protection. SMS codes and authenticator apps are far better than passwords alone, but they can still be phished. Hardware keys and passkeys are in a different league — they're resistant to phishing by design.

This page helps you decide which MFA methods to deploy, where to prioritize, and what to push toward over time.

---

## 2. The Comparison Matrix

| Method | Phishing Resistance | User Friction | Per-User Cost | SMB Suitability | Best For |
|--------|-------------------|---------------|--------------|----------------|----------|
| **SMS / Text Message** | Low | Low | Free | Good (easy to deploy, but weakest MFA option) | Legacy systems that don't support better options |
| **Voice Call** | Low | Medium | Free | Limited (same weaknesses as SMS, more disruptive) | Accessibility backup only |
| **Email OTP** | Low | Low | Free | Limited (if email is compromised, MFA is bypassed) | Low-risk internal tools only |
| **Authenticator App (TOTP)** | Medium | Low | Free | Excellent (strong baseline for most SMBs) | Default MFA for most employees and services |
| **Push Notification** | Medium | Very Low | Free–$6/user/mo | Excellent (fast and easy, watch for push fatigue) | Day-to-day authentication for most staff |
| **Number Matching Push** | Medium–High | Low | Free–$6/user/mo | Excellent (significantly reduces push fatigue attacks) | Recommended upgrade from basic push |
| **Hardware Security Key (FIDO2)** | Very High | Medium | $25–$70/key | Good (strong protection, moderate cost, key management required) | Admins, executives, finance, and high-risk roles |
| **Passkeys (device-bound)** | Very High | Very Low | Free | Excellent (no cost, built into modern devices) | Emerging standard — deploy wherever supported |
| **Passkeys (synced)** | High | Very Low | Free | Excellent (convenient, but syncing introduces some risk) | Consumer and lower-sensitivity business accounts |
| **Smart Card / PIV** | Very High | High | $50–$150/card + reader | Limited (complex deployment, typically government/enterprise) | Regulated industries, government contractors |
| **Certificate-Based Auth** | Very High | High (initial setup) | Varies (PKI infrastructure) | Limited (requires PKI — overkill for most SMBs) | Large enterprises with existing PKI |

---

## 3. Understanding Phishing Resistance

Not all MFA stops phishing. Here's why it matters.

A **phishable** MFA method is one where an attacker can trick you into handing over your second factor. The classic attack: you get a fake login page that looks exactly like Microsoft 365. You enter your password and your SMS code. The attacker relays both to the real site in real time and takes over your session. This is called an adversary-in-the-middle (AitM) attack, and it works against SMS, email OTP, TOTP authenticator apps, and even basic push notifications.

A **phishing-resistant** MFA method is one where the second factor is cryptographically bound to the real website. Hardware security keys and passkeys use the FIDO2/WebAuthn protocol, which checks the domain of the site you're logging into. If you're on a fake site, the key simply won't work — there's nothing for you to accidentally hand over. The authentication happens between the key and the legitimate server, and a fake site can't intercept it.

### What "phishing-resistant" actually means

| Rating | What it means | Methods |
|--------|--------------|---------|
| **Low** | Can be intercepted in real-time by an attacker-controlled proxy. Your code or approval goes straight to the attacker. | SMS, voice call, email OTP |
| **Medium** | Harder to intercept than SMS but still vulnerable to real-time phishing proxies and social engineering (e.g., push fatigue attacks where the attacker sends repeated prompts until you approve one). | TOTP authenticator apps, basic push notifications |
| **Medium–High** | Resists most automated attacks. Number matching requires you to type a specific number from the login screen, which makes blind approval much harder — but a sophisticated real-time proxy can still relay the number. | Number matching push |
| **High** | Cryptographically bound to the real site. Synced passkeys add a small risk if the sync mechanism is compromised, but the authentication itself is phishing-resistant. | Synced passkeys |
| **Very High** | Cryptographically bound to the real site and to a specific physical device. Nothing to type, nothing to relay, nothing to approve on a different screen. The key talks directly to the legitimate server. | Hardware security keys (FIDO2), device-bound passkeys, smart cards, certificate-based auth |

---

## 4. Method-by-Method Breakdown

### SMS / Text Message

How it works: You receive a 6-digit code via text message and type it into the login screen.

**Strengths:** Universal — works on any phone, no app required. Easy to deploy. Users already understand it.

**Weaknesses:** Vulnerable to SIM swapping (an attacker convinces your carrier to transfer your number to their SIM), SS7 network interception, and real-time phishing proxies. NIST has flagged SMS as a "restricted" authenticator since 2017, meaning it should only be used when no better option is available.

**The reality for SMBs:** SMS is still better than no MFA. If the choice is SMS or nothing, use SMS. But don't treat it as your long-term answer — plan to move admin accounts and high-risk users to authenticator apps or hardware keys as soon as practical.

### Authenticator App (TOTP)

How it works: An app (Microsoft Authenticator, Google Authenticator, Authy, etc.) generates a new 6-digit code every 30 seconds. You type the current code into the login screen.

**Strengths:** Free. Works offline. No phone number needed. Significantly harder to intercept than SMS — an attacker would need access to your device or your TOTP secret.

**Weaknesses:** Still phishable by real-time proxy attacks. If you type your TOTP code into a fake site, the attacker can relay it to the real site before it expires. Also, if users don't back up their TOTP secrets, losing a phone means losing access to every account.

**The reality for SMBs:** This is the practical baseline for most companies. It's free, it works with almost everything, and it's a massive improvement over passwords alone. Deploy this for all users and all services that support it.

### Push Notification

How it works: When you log in, the authentication service sends a push notification to your phone. You tap "Approve" to complete the login.

**Strengths:** Fast and easy — no codes to type. Built into Microsoft Authenticator, Duo, Okta Verify, and others.

**Weaknesses:** Vulnerable to "push fatigue" or "MFA bombing" — an attacker who has your password can send repeated push requests until you accidentally (or frustratedly) tap Approve. This is a real, documented attack method used in major breaches.

**The fix:** Use **number matching** (also called "number challenge"). Instead of a simple Approve/Deny prompt, the login screen shows a two-digit number and you have to type that number into the push notification. This makes it much harder for an attacker to get you to approve a request you didn't initiate. Microsoft enabled number matching by default for Authenticator push notifications in May 2023.

### Hardware Security Key (FIDO2)

How it works: A physical USB or NFC device (YubiKey, Google Titan Key, Feitian, etc.) that you plug in or tap when prompted during login. The key performs a cryptographic handshake with the service — it checks the domain, generates a unique response, and never sends a reusable secret.

**Strengths:** Phishing-resistant by design. Nothing to type, nothing to relay. An attacker with your password and a perfect phishing page still can't get in because the key won't respond to a fake domain. No batteries, no network connection needed.

**Weaknesses:** You have to buy them ($25–$70 per key, and each user should have two — one primary, one backup). Users can lose them. Not all services support FIDO2 yet (though coverage is growing fast). Requires some IT setup and a process for lost key replacement.

**The reality for SMBs:** Start with your highest-risk accounts: IT admins, executives, finance team, and anyone with access to sensitive client data. The cost of a few YubiKeys is trivial compared to the cost of a single compromised admin account. Google reported that after deploying hardware keys to all 85,000+ employees, they had zero successful phishing attacks on employee accounts.

### Passkeys

How it works: Passkeys are the next evolution of FIDO2. Instead of a separate physical key, the credential lives on your device — your phone, laptop, or tablet. Authentication uses biometrics (Face ID, fingerprint, Windows Hello) or your device PIN. The cryptographic protocol is the same as hardware keys: domain-bound, phishing-resistant, nothing to type or relay.

**Device-bound passkeys** stay on one device and can't be copied. They work like a built-in hardware key.

**Synced passkeys** are backed up and synced across your devices through your platform's cloud (Apple iCloud Keychain, Google Password Manager, or a password manager like 1Password or Bitwarden). This means you don't lose access if you lose a single device — but it also means the passkey's security is partially tied to the security of your cloud account.

**Strengths:** Free. Built into modern operating systems and browsers. No hardware to buy or carry. The user experience is often faster than typing a password — you just scan your fingerprint or face.

**Weaknesses:** Platform support is still rolling out. Not all services support passkeys yet. Cross-platform use can be clunky (e.g., using an iPhone passkey to log in on a Windows machine). Synced passkeys inherit the security of your cloud account — if your iCloud or Google account is compromised, your synced passkeys could be too. Enterprise management tools for passkeys are still maturing.

**The reality for SMBs:** Start deploying passkeys wherever they're supported — Microsoft, Google, Apple, and many SaaS services already support them. For consumer-facing accounts and lower-sensitivity business accounts, synced passkeys are excellent. For admin and high-risk accounts, device-bound passkeys or hardware keys are the better choice until enterprise passkey management matures.

---

## 5. What This Means for Your Company

### The practical deployment path for most SMBs

**Phase 1 — Get everyone on MFA (now).** If you still have accounts without MFA, fix that first. Authenticator apps (TOTP) or push notifications with number matching are the right default for most employees. This alone stops the vast majority of account compromise attacks.

**Phase 2 — Protect your highest-risk accounts with phishing-resistant MFA.** IT admins, executives, finance team, and anyone with access to sensitive client data should use hardware security keys or device-bound passkeys. These accounts are the ones attackers target first, and a compromised admin account can take down the entire company.

**Phase 3 — Deploy passkeys broadly as support matures.** As more services support passkeys and enterprise management tools improve, start moving your general workforce to passkeys. The user experience is better than TOTP, the security is stronger, and there's no per-user cost.

**Phase 4 — Phase out SMS.** Once your users are on authenticator apps, push, or passkeys, disable SMS as an MFA option for all accounts that support better methods. Keep it only as a last resort for legacy systems that don't support anything else.

### Don't let perfect be the enemy of good

If deploying hardware keys to everyone isn't realistic right now, that's fine. An authenticator app on every account is still a massive security improvement. The goal is to move up the phishing resistance ladder over time — not to wait at the bottom until you can afford to jump to the top.

---

## 6. Quick Reference: MFA Support by Common Platforms

| Platform | TOTP | Push | FIDO2 Keys | Passkeys | SMS (as backup) |
|----------|------|------|-----------|----------|----------------|
| Microsoft 365 / Entra ID | Yes | Yes (Authenticator) | Yes | Yes (preview/rolling out) | Yes |
| Google Workspace | Yes | Yes (Google Prompt) | Yes | Yes | Yes |
| Apple (iCloud, managed Apple IDs) | Yes | Yes (trusted device) | Yes | Yes | Yes |
| Salesforce | Yes | Yes (Salesforce Authenticator) | Yes | Yes | Yes |
| Slack | Yes | No | No | No | Yes |
| Zoom | Yes | No | No | No | Yes |
| QuickBooks Online | Yes | Yes (Intuit push) | No | No | Yes |
| Dropbox Business | Yes | No | Yes | Yes | Yes |
| GitHub | Yes | No | Yes | Yes | Yes |
| AWS | Yes | No | Yes | Yes | Yes (virtual MFA) |

*This table reflects capabilities as of March 2026. Platform support for passkeys and FIDO2 is expanding rapidly — check your vendor's current documentation.*

---

## 7. Sources and Further Reading

### NIST

- [NIST SP 800-63B Revision 4 — Digital Identity Guidelines: Authentication and Lifecycle Management](https://pages.nist.gov/800-63-4/sp800-63b.html) — Sections on authenticator types and phishing resistance

### FIDO Alliance

- [FIDO Alliance: How FIDO Works](https://fidoalliance.org/how-fido-works/) — Overview of FIDO2/WebAuthn protocol
- [Passkeys.dev](https://passkeys.dev/) — Developer and user resources for passkey adoption

### Microsoft

- [Microsoft Entra ID: Authentication Methods](https://learn.microsoft.com/en-us/entra/identity/authentication/concept-authentication-methods) — Detailed guide to all supported MFA methods
- [Microsoft: Phishing-Resistant MFA](https://learn.microsoft.com/en-us/entra/identity/authentication/concept-authentication-strengths) — Authentication strengths and conditional access policies

### CISA

- [CISA: Implementing Phishing-Resistant MFA](https://www.cisa.gov/sites/default/files/publications/fact-sheet-implementing-phishing-resistant-mfa-508c.pdf) — Federal guidance applicable to any organization
- [CISA: More Than a Password](https://www.cisa.gov/MFA) — General MFA guidance

### Google

- [Google Security Blog: Security Keys Neutralized Phishing](https://security.googleblog.com/2019/05/new-research-how-effective-is-basic.html) — Google's experience deploying hardware keys to 85,000+ employees

---

## 8. Revision History

| Version | Date | Summary |
|---------|------|---------|
| 1.0 | March 2026 | Initial release |

---

*This reference is part of the [Open IT Policy Library](https://github.com/sortedsol/Open-IT-Policy-Library) by [Sorted Solution](https://www.sortedsolution.com). Free to use, fork, and adapt. Attribution appreciated.*
