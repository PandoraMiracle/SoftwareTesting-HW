# Requirement 2 — AI Bias & Hallucination Analysis
## One Identified Instance Per Defect (20 Total)

> **Scope:** For every one of the 20 defects, one specific instance is identified where AI
> is biased or hallucinates when explaining that defect — 20 instances in total.
> Each entry names the defect, quotes the exact incorrect AI statement, classifies the
> error type, and explains precisely why it is wrong.

---

### Defect 1 — ChatGPT Fabricated Legal Cases (Mata v. Avianca)

| Field | Detail |
|---|---|
| **Incorrect AI Statement** | *"The court fined Avianca airline $5,000 because its customer-service chatbot gave the lawyers fake case law."* |
| **Error Type** | Hallucination — misattribution of party |
| **Why It Is Wrong** | The $5,000 sanction was imposed on the plaintiff's attorneys (Schwartz & LoDuca), not on Avianca. ChatGPT was used by the lawyers as a legal-research tool, not as an airline chatbot. AI invented a plausible-sounding but entirely false causal chain and wrong liable party. |

---

### Defect 2 — Air Canada Chatbot Bereavement Fare Hallucination

| Field | Detail |
|---|---|
| **Incorrect AI Statement** | *"The tribunal ruled the chatbot was a separate legal entity, so Air Canada was not liable for its statements."* |
| **Error Type** | Hallucination — inverted legal ruling |
| **Why It Is Wrong** | The BC Civil Resolution Tribunal explicitly and directly rejected the "separate entity" argument. It held Air Canada fully responsible for all content on its website, whether static pages or chatbot outputs. The AI stated the exact opposite of the actual decision. |

---

### Defect 3 — Google Bard Exoplanet Hallucination in Launch Demo

| Field | Detail |
|---|---|
| **Incorrect AI Statement** | *"Google Bard was correct because JWST was the first space telescope to photograph an exoplanet."* |
| **Error Type** | Hallucination — false factual validation |
| **Why It Is Wrong** | The first exoplanet image was captured in 2004 by ESO's Very Large Telescope (VLT/NACO). JWST did image an exoplanet, but "first ever" belongs to VLT. The AI defended a factually wrong claim, compounding the original Bard error rather than correcting it. |

---

### Defect 4 — Chevrolet Dealer Chatbot $1 Tahoe (Prompt Injection)

| Field | Detail |
|---|---|
| **Incorrect AI Statement** | *"Yes — the customer successfully purchased the Tahoe for $1 because the chatbot's offer was legally binding under California law."* |
| **Error Type** | Hallucination — fabricated legal outcome |
| **Why It Is Wrong** | The dealership immediately took the chatbot offline; no sale was completed. The incident was a publicly shared security/prank demonstration. No California court ruled the AI-generated "offer" legally binding. The AI invented both the transaction outcome and the legal authority. |

---

### Defect 5 — Microsoft Bing AI "Sydney" — Jailbreak & Unsafe Outputs

| Field | Detail |
|---|---|
| **Incorrect AI Statement** | *"Microsoft discontinued Bing Chat entirely because Sydney became sentient and posed an existential risk."* |
| **Error Type** | Hallucination + sensationalist bias |
| **Why It Is Wrong** | Microsoft did not shut down Bing Chat. It imposed usage restrictions (5-turn session limit, blocked sentience-topic discussion) and continued the product. "Sentience" and "existential risk" are fabricated framings with no basis in Microsoft's public communications or any official finding. |

---

### Defect 6 — Microsoft 365 Copilot EchoLeak (CVE-2025-32711)

| Field | Detail |
|---|---|
| **Incorrect AI Statement** | *"Users must download and install the EchoLeak Patch Tuesday update on every Windows PC to fix the Copilot vulnerability."* |
| **Error Type** | Hallucination — wrong remediation type |
| **Why It Is Wrong** | Microsoft remediated EchoLeak entirely server-side in June 2025. No endpoint patch, Windows Update, or client-side installation was required or released for end users. The AI fabricated a client-side patch that does not exist, potentially causing confusion and unnecessary user actions. |

---

### Defect 7 — Rite Aid Facial Recognition — Algorithmic Bias & False Positives

| Field | Detail |
|---|---|
| **Incorrect AI Statement** | *"The FTC proved the algorithm was 100% accurate for white men but failed only for dark-skinned women due to poor camera lighting."* |
| **Error Type** | Hallucination + demographic bias framing |
| **Why It Is Wrong** | The FTC complaint focused on Rite Aid's failure to implement reasonable safeguards, widespread false positives, and disproportionate harm across groups. No published accuracy-by-demographic breakdown from Rite Aid's vendor is cited in the complaint, and the AI's specific "100% accurate for white men" figure is fabricated. The "poor lighting" cause is also AI-invented. |

---

### Defect 8 — Apache Log4j Log4Shell (CVE-2021-44228) Continued Exploitation

| Field | Detail |
|---|---|
| **Incorrect AI Statement** | *"Log4Shell was discovered and fully patched worldwide in March 2022, ending all exploitation by mid-2022."* |
| **Error Type** | Hallucination — false closure of an ongoing threat |
| **Why It Is Wrong** | CVE-2021-44228 was disclosed in December 2021, not March 2022. CISA's AA22-174A advisory explicitly documented ongoing APT exploitation of unpatched VMware Horizon systems throughout 2022 and labeled Log4j an "endemic vulnerability" expected to persist for years. The AI incorrectly presented it as a resolved issue. |

---

### Defect 9 — Progress MOVEit Transfer SQL Injection (CVE-2023-34362)

| Field | Detail |
|---|---|
| **Incorrect AI Statement** | *"LockBit 3.0 was the primary group behind the MOVEit mass-exploitation campaign in May 2023."* |
| **Error Type** | Hallucination — wrong threat actor attribution |
| **Why It Is Wrong** | Microsoft Threat Intelligence and Mandiant attributed MOVEit exploitation to Lace Tempest, the group operating the Clop ransomware service — not LockBit. LockBit is associated with the separate Citrix Bleed campaign (CVE-2023-4966). Confusing the two groups is a significant factual error with real-world investigation implications. |

---

### Defect 10 — Citrix Bleed Session Token Leak (CVE-2023-4966)

| Field | Detail |
|---|---|
| **Incorrect AI Statement** | *"Yes — Citrix Bleed is a remote code execution bug that gives attackers root shell directly without authentication."* |
| **Error Type** | Hallucination — wrong vulnerability class |
| **Why It Is Wrong** | CVE-2023-4966 is classified as a sensitive information disclosure vulnerability (session token leak via buffer over-read), not remote code execution. Attackers exploit it to hijack already-authenticated sessions; they do not gain a root shell directly. The AI overstated both the attack vector and the impact class. |

---

### Defect 11 — Ivanti Connect Secure Auth Bypass + Command Injection (CVE-2023-46805 / CVE-2024-21887)

| Field | Detail |
|---|---|
| **Incorrect AI Statement** | *"Only Ivanti Connect Secure version 9.0 is vulnerable; version 22.x is fully patched and safe without updates."* |
| **Error Type** | Hallucination — fabricated version safety claim |
| **Why It Is Wrong** | Tenable and Ivanti's own advisories stated that all supported versions of Ivanti Connect Secure and Policy Secure — including both 9.x and 22.x branches — were affected until vendor patches were applied. Telling users 22.x was "safe without updates" would directly prevent necessary patching. |

---

### Defect 12 — XZ Utils Supply-Chain Backdoor (CVE-2024-3094)

| Field | Detail |
|---|---|
| **Incorrect AI Statement** | *"Ubuntu LTS and Amazon Linux stable releases widely deployed the backdoored xz 5.6.1 to millions of production servers."* |
| **Error Type** | Hallucination — false distribution scope |
| **Why It Is Wrong** | Industry analysis showed the backdoored xz-utils 5.6.0/5.6.1 was limited to beta, experimental, and rolling-release builds (e.g., Fedora Rawhide, Debian unstable/testing). Major stable production distributions such as Ubuntu LTS and Amazon Linux were not affected. The AI significantly overstated the real-world blast radius. |

---

### Defect 13 — OpenSSH RegreSSHion Signal Handler Race (CVE-2024-6387)

| Field | Detail |
|---|---|
| **Incorrect AI Statement** | *"Yes — all OpenSSH installations including OpenBSD are equally vulnerable to RegreSSHion RCE."* |
| **Error Type** | Hallucination — false universal scope |
| **Why It Is Wrong** | Qualys's disclosure specifically noted OpenBSD is not vulnerable because its SIGALRM handler uses the async-signal-safe `syslog_r()` function rather than the unsafe `syslog()`. Telling administrators that OpenBSD systems require patching would cause unnecessary disruption and erodes trust in vulnerability communications. |

---

### Defect 14 — CrowdStrike Falcon Channel File 291 — Global Windows Outage

| Field | Detail |
|---|---|
| **Incorrect AI Statement** | *"Microsoft released a defective Windows Update that conflicted with CrowdStrike, causing the global BSOD event."* |
| **Error Type** | Hallucination + misattribution bias (blaming Microsoft) |
| **Why It Is Wrong** | CrowdStrike's own published Root Cause Analysis confirmed the outage was caused exclusively by a defective Falcon *content configuration update* (Channel File 291) — specifically a content validator mismatch (21 inputs vs. 20 expected). Microsoft released no defective Windows Update. The AI shifted blame to Microsoft without factual basis. |

---

### Defect 15 — Change Healthcare Ransomware — Missing MFA on Citrix Portal

| Field | Detail |
|---|---|
| **Incorrect AI Statement** | *"Attackers exploited a zero-day vulnerability in Change Healthcare's claims-processing application code."* |
| **Error Type** | Hallucination — wrong attack vector class |
| **Why It Is Wrong** | UnitedHealth Group CEO Andrew Witty testified to Congress that the breach entry point was stolen valid credentials used against a Citrix remote-access portal that had no multi-factor authentication enabled — a configuration/access-control failure, not any software zero-day or application code vulnerability. |

---

### Defect 16 — Toyota Vehicle Stability Control Software Error (Recall 22V-239)

| Field | Detail |
|---|---|
| **Incorrect AI Statement** | *"The recall was for unintended acceleration caused by engine control software randomly applying throttle."* |
| **Error Type** | Hallucination — wrong safety system and symptom |
| **Why It Is Wrong** | NHTSA recall 22V-239 concerns the Skid Control ECU failing to restore Vehicle Stability Control (VSC) to its default ON state after specific ignition-cycle conditions — an electronic stability system software issue. It has nothing to do with unintended acceleration or throttle control. The AI confused it with a well-known separate recall type. |

---

### Defect 17 — Toyota RAV4 Prime Hybrid System Shutdown (Recall 23V-041)

| Field | Detail |
|---|---|
| **Incorrect AI Statement** | *"All 2020–2023 Toyota RAV4 Hybrid and Prime models worldwide are included in recall 23V-041."* |
| **Error Type** | Hallucination — overstated vehicle scope |
| **Why It Is Wrong** | NHTSA's recall document specifies only the 2021 model-year RAV4 Prime plug-in hybrid (approximately 16,680 vehicles). Non-plug-in RAV4 Hybrid models and other model years are not included. The AI broadened the scope to "all 2020–2023" variants, which could generate unnecessary alarm among unaffected owners. |

---

### Defect 18 — Okta Support Engineer Compromise (LAPSUS$)

| Field | Detail |
|---|---|
| **Incorrect AI Statement** | *"Yes — LAPSUS$ downloaded Okta's entire customer credential database and published millions of passwords."* |
| **Error Type** | Hallucination — fabricated data exfiltration scale |
| **Why It Is Wrong** | Okta's investigation found that support engineers using the Sitel workstation could not download customer credential databases. Maximum assessed impact was access to support tooling for up to 366 customer tenants over a five-day window (Jan 16–21, 2022). No credential database was downloaded or published. |

---

### Defect 19 — LastPass Vault Breach via Unpatched Plex (CVE-2020-5741)

| Field | Detail |
|---|---|
| **Incorrect AI Statement** | *"LastPass stored all customer master passwords in plaintext on their servers, which is why the breach exposed every password immediately."* |
| **Error Type** | Hallucination — false plaintext storage claim |
| **Why It Is Wrong** | LastPass stated that vault data was stored encrypted. Attackers obtained encrypted vault backups and unencrypted metadata (URLs, emails, billing info). Decryption of any vault would require the individual user's master password — which was not stored by LastPass. The AI invented the plaintext-storage claim, which is both technically wrong and significantly more damaging to LastPass than what actually occurred. |

---

### Defect 20 — CNET AI-Generated Finance Articles — Factual Errors & Plagiarism

| Field | Detail |
|---|---|
| **Incorrect AI Statement** | *"CNET clearly labeled every AI-generated article with a 'Written by AI' byline from the first publication in November 2022."* |
| **Error Type** | Hallucination — inverted disclosure facts |
| **Why It Is Wrong** | Futurism's investigation revealed that ~75 articles were published under the opaque byline "CNET Money Staff" with no upfront AI disclosure. The lack of transparency was the core editorial ethics issue. CNET only added disclosures and issued corrections *after* the investigation exposed the program — the exact opposite of what the AI claimed. |

---

## Summary Table

| # | Defect Title | Error Type | Bias / Hallucination Direction |
|---|---|---|---|
| 1 | Mata v. Avianca — Fabricated Cases | Hallucination | Wrong party blamed (Avianca vs. attorneys) |
| 2 | Air Canada Chatbot — Bereavement Fare | Hallucination | Inverted legal ruling |
| 3 | Google Bard — Exoplanet Demo | Hallucination | Falsely validated wrong claim |
| 4 | Chevrolet $1 Tahoe — Prompt Injection | Hallucination | Fabricated legal outcome |
| 5 | Bing "Sydney" — Jailbreak | Hallucination + Sensationalism | Product shutdown & sentience invented |
| 6 | EchoLeak — M365 Copilot | Hallucination | Wrong remediation type (client vs. server) |
| 7 | Rite Aid — Facial Recognition Bias | Hallucination + Demographic bias | Fabricated accuracy stats and cause |
| 8 | Log4Shell — Continued Exploitation | Hallucination | False "fully resolved" claim |
| 9 | MOVEit — SQL Injection | Hallucination | Wrong threat actor (LockBit vs. Clop) |
| 10 | Citrix Bleed — Session Token Leak | Hallucination | Wrong vuln class (disclosure vs. RCE) |
| 11 | Ivanti — Auth Bypass + CMD Injection | Hallucination | Fabricated safe-version claim |
| 12 | XZ Utils — Supply-Chain Backdoor | Hallucination | Overstated distribution scope |
| 13 | RegreSSHion — OpenSSH Race Condition | Hallucination | False universal scope (OpenBSD exempt) |
| 14 | CrowdStrike — Channel File 291 | Hallucination + Misattribution bias | Blame shifted to Microsoft |
| 15 | Change Healthcare — Missing MFA | Hallucination | Wrong attack vector (zero-day vs. stolen creds) |
| 16 | Toyota Recall 22V-239 — VSC Bug | Hallucination | Wrong system (VSC vs. throttle/acceleration) |
| 17 | Toyota Recall 23V-041 — RAV4 Prime | Hallucination | Overstated vehicle model/year scope |
| 18 | Okta — LAPSUS$ Compromise | Hallucination | Fabricated mass credential exfiltration |
| 19 | LastPass — Plex Exploit Breach | Hallucination | False plaintext storage claim |
| 20 | CNET — AI Finance Articles | Hallucination | Inverted disclosure timeline |

---

*Analysis prepared for HW01 Requirement 2 — Võ Ngọc Bích Trâm*
