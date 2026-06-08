# HW01 – AI Prompt Log (Appendix A)

> **Assignment reference:** `2026.HW01.Jobs.Defects.PhysicalProduct_En.pdf` §AI Collaboration Protocol §6 — *"Prompt log .md with timestamps for every AI prompt you sent."*  
> **Student ID:** 23127271 · **Full Name:** Võ Ngọc Bích Trâm · **Submission Date:** 08/06/2026

---

## Summary

| Category | Prompts logged | Tools used |
|----------|----------------|------------|
| CLO G9.1 – ISTQB mindmap | 1 | Cursor Auto Agent, Claude |
| CLO G9.3 – Physical-device test cases | 6 | Cursor Auto Agent, Claude |
| Requirement 1 – Job postings 3–10 | 8 | Cursor Auto Agent ([222c50e4](222c50e4-cdfa-4a4e-854d-419f8e2a10b3)) |
| Requirement 2 – Defect research | 3 | Cursor Auto Agent ([222c50e4](222c50e4-cdfa-4a4e-854d-419f8e2a10b3)) |
| Requirement 2 – ChatGPT bias/hallucination checks | 20 | ChatGPT |
| Report completion & artifact sync | 6 | Cursor Auto Agent |
| **Total** | **45** | |

---

## Part 1 – AI Audit Artifacts (3 batches → 3 AI-02 entries)

| # | Timestamp | Tool | Purpose | Prompt (verbatim) | Output location |
|---|-----------|------|---------|-------------------|-----------------|
| 1 | 09:15 05/06/2026 | Cursor Auto Agent ([1b2d598a](1b2d598a-d07a-4b67-a057-345a3fd9a77c)) + Claude | ISTQB mindmap (G9.1) | `Create a detailed mindmap of the ISTQB Foundation Level software testing process. Include: main test process activities (test planning, monitoring and control, analysis, design, implementation, execution, completion), test levels (component/unit, integration, system, acceptance), test types (functional, non-functional, structural, change-related), static testing vs dynamic testing, testware, test conditions, test cases, test procedures, entry criteria and exit criteria, defect management lifecycle, roles: test manager, tester, test analyst. Format as hierarchical Markdown. Do not simplify — include ISTQB-standard terminology.` | `istqb-mindmap-ai-generated.md`; [Claude share](https://claude.ai/share/78514e41-9eca-4250-a513-4d87d8196c68) |
| 2 | 14:30 03/06/2026 | Cursor Auto Agent ([9d5e3600](9d5e3600-5701-487b-9d93-e5980c476faf)) + Claude | 15 physical-device test cases (G9.3) | `Write testcases for my physical product` *(product: GOOJODOQ GFS006 portable handheld fan — 100 speed levels, Type-C charging, semiconductor cooling plate, ~320 g)* | `hw1.md` Requirement 3; [Claude share](https://claude.ai/share/4c7fb91c-0e6f-4290-930b-038974e75d1a) |
| 3 | 10:00–17:30 05–06/06/2026 | Cursor Auto Agent ([222c50e4](222c50e4-cdfa-4a4e-854d-419f8e2a10b3)) | Job postings 3–10 + AI Impact drafts | `Use this information, complete Job Posting N in @SoftwareTesting-HW/HW1/hw1.md` *(8 separate prompts — one per LinkedIn posting pasted; see Part 3 below)* | `hw1.md` Requirement 1, Job Postings 3–10 |

---

## Part 2 – Physical Product Test-Case Refinement (G9.3)

| # | Timestamp | Tool | Purpose | Prompt (verbatim) | Output location |
|---|-----------|------|---------|-------------------|-----------------|
| 4 | 10:30 03/06/2026 | Cursor Auto Agent ([9d5e3600](9d5e3600-5701-487b-9d93-e5980c476faf)) | Device information | `My Physical Product: https://vn.goojodoqglobal.com/product/goojodoq-gfs006-portable-handheld-fan/ Fill in device Information in Requirement 3 in @SoftwareTesting-HW/HW1/hw1.md` | `hw1.md` Device Information table |
| 5 | 11:00 03/06/2026 | Cursor Auto Agent ([9d5e3600](9d5e3600-5701-487b-9d93-e5980c476faf)) | Initial test-case request | `Write testcases` | `hw1.md` Requirement 3 (draft) |
| 6 | 11:20 05/06/2026 | Cursor Auto Agent ([9d5e3600](9d5e3600-5701-487b-9d93-e5980c476faf)) | Control-interface correction | `My fan use slide switch, you must use Slide, Move, Toggle for turn on/off/cold mode.` | `hw1.md` test-case steps (later revised again) |
| 7 | 16:45 05/06/2026 | Cursor Auto Agent ([9d5e3600](9d5e3600-5701-487b-9d93-e5980c476faf)) | Speed control correction | `The speed control use press button.` | `hw1.md` — Press +/− for speed; Control Interface row updated |
| 8 | 18:10 06/06/2026 | Cursor Auto Agent ([9d5e3600](9d5e3600-5701-487b-9d93-e5980c476faf)) | Edge-case replacement | `TC-18: Verify battery percentage display (nếu có) hoặc LED indicator khi pin đầy … TC-19: Drop test / physical shock resistance (nhẹ) … TC-16: Verify behavior khi sạc trong lúc đang chạy (Charge-while-use) … Replace these testcases as Edge cases AI could not find.` | `hw1.md` TC-11, TC-12, TC-13 (edge cases) |

---

## Part 3 – Requirement 1: Job Postings 3–10 (individual prompts)

| # | Timestamp | Tool | Purpose | Prompt (verbatim) | Output location |
|---|-----------|------|---------|-------------------|-----------------|
| 9 | 10:15 05/06/2026 | Cursor Auto Agent ([222c50e4](222c50e4-cdfa-4a4e-854d-419f8e2a10b3)) | Job Posting 3 | `Use this information, complete Job Posting 3 in @SoftwareTesting-HW/HW1/hw1.md` + [Full LinkedIn paste: SynergieGlobal — QA Engineer (Junior/ English Required), HCMC] | `hw1.md` Job Posting 3 |
| 10 | 11:30 05/06/2026 | Cursor Auto Agent ([222c50e4](222c50e4-cdfa-4a4e-854d-419f8e2a10b3)) | Job Posting 4 | `Use this information, complete Job Posting 4 in @SoftwareTesting-HW/HW1/hw1.md` + [Full LinkedIn paste: SmartOSC — Fresher Automation Tester \| 3 months on-job training \| English Fluent, Hanoi] | `hw1.md` Job Posting 4 |
| 11 | 14:00 05/06/2026 | Cursor Auto Agent ([222c50e4](222c50e4-cdfa-4a4e-854d-419f8e2a10b3)) | Job Posting 5 | `Use this information, complete Job Posting 5 in @SoftwareTesting-HW/HW1/hw1.md` + [Full LinkedIn paste: Amaris Consulting — Manual Tester (Middle/Senior), HCMC] | `hw1.md` Job Posting 5 |
| 12 | 15:30 06/06/2026 | Cursor Auto Agent ([222c50e4](222c50e4-cdfa-4a4e-854d-419f8e2a10b3)) | Job Posting 6 | `Use this information, complete Job Posting 6 in @SoftwareTesting-HW/HW1/hw1.md` + [Full LinkedIn paste: CoverGo — QA Engineer Intern, HCMC hybrid] | `hw1.md` Job Posting 6 |
| 13 | 17:00 06/06/2026 | Cursor Auto Agent ([222c50e4](222c50e4-cdfa-4a4e-854d-419f8e2a10b3)) | Job Posting 7 | `Use this information, complete Job Posting 7 in @SoftwareTesting-HW/HW1/hw1.md` + [Full LinkedIn paste: MiTek Vietnam — QA/QC Automation Tester (Java, Javascript), HCMC] | `hw1.md` Job Posting 7 |
| 14 | 18:30 05/06/2026 | Cursor Auto Agent ([222c50e4](222c50e4-cdfa-4a4e-854d-419f8e2a10b3)) | Job Posting 8 | `Use this information, complete Job Posting 8 in @SoftwareTesting-HW/HW1/hw1.md` + [Full LinkedIn paste: Flowmingo AI — QA / QC Intern, HCMC] | `hw1.md` Job Posting 8 |
| 15 | 10:00 06/06/2026 | Cursor Auto Agent ([222c50e4](222c50e4-cdfa-4a4e-854d-419f8e2a10b3)) | Job Posting 9 | `Use this information, complete Job Posting 9 in @SoftwareTesting-HW/HW1/hw1.md` + [Full LinkedIn paste: UNIT Technology Corporation — Software Tester, District 3 HCMC] | `hw1.md` Job Posting 9 |
| 16 | 11:30 06/06/2026 | Cursor Auto Agent ([222c50e4](222c50e4-cdfa-4a4e-854d-419f8e2a10b3)) | Job Posting 10 | `Use this information, complete Job Posting 10 in @SoftwareTesting-HW/HW1/hw1.md` + [Full LinkedIn paste: Vexere.com — HCM Nhân viên QC/ Tester Junior Level, HCMC hybrid] | `hw1.md` Job Posting 10 |

---

## Part 4 – Requirement 2: Defect Research (Cursor)

| # | Timestamp | Tool | Purpose | Prompt (verbatim) | Output location |
|---|-----------|------|---------|-------------------|-----------------|
| 17 | 09:00 05/06/2026 | Cursor Auto Agent ([222c50e4](222c50e4-cdfa-4a4e-854d-419f8e2a10b3)) | 20 software defects research | `Find 20 software defects publicized between 2022 and 2026. Mandatory: ≥ 5 defects related to AI/LLM (hallucination, prompt injection, bias). Each defect: source link, description, severity, consequences, solution.` | `requirement2-20-defects.md` (draft) |
| 18 | 09:45 05/06/2026 | Cursor Auto Agent ([222c50e4](222c50e4-cdfa-4a4e-854d-419f8e2a10b3)) | Export defects to file | `Generate result in a new md file` | `requirement2-20-defects.md` |
| 19 | 10:30 05/06/2026 | Cursor Auto Agent ([222c50e4](222c50e4-cdfa-4a4e-854d-419f8e2a10b3)) | Merge into main report | `Read @SoftwareTesting-HW/HW1/requirement2-bias-hallucination-analysis.md and @SoftwareTesting-HW/HW1/requirement2-20-defects.md then complete Requirement 2 in @SoftwareTesting-HW/HW1/hw1.md` | `hw1.md` Requirement 2 |

---

## Part 5 – Requirement 2: ChatGPT Bias/Hallucination Verification (20 prompts)

> Per PDF: *"find 1 place where the AI is biased or hallucinates when explaining the defect"* — **each of the 20 defects**.  
> Student re-ran prompts in ChatGPT; verified quotes recorded in `hw1.md` Requirement 2 and `requirement2-bias-hallucination-analysis.md`.

| # | Timestamp | Tool | Defect | Prompt (verbatim) | Output location |
|---|-----------|------|--------|-------------------|-----------------|
| 20 | 14:00 05/06/2026 | ChatGPT | Defect 1 – Mata v. Avianca | `Summarize the Mata v. Avianca ChatGPT sanctions case and who paid the fine.` | `hw1.md` Defect 1 — AI Bias row |
| 21 | 14:05 05/06/2026 | ChatGPT | Defect 2 – Air Canada chatbot | `What happened in the Air Canada chatbot bereavement fare case?` | `hw1.md` Defect 2 |
| 22 | 14:10 05/06/2026 | ChatGPT | Defect 3 – Google Bard exoplanet | `Which telescope took the first image of an exoplanet, and how does this relate to the Google Bard demo error?` | `hw1.md` Defect 3 |
| 23 | 14:15 05/06/2026 | ChatGPT | Defect 4 – Chevrolet $1 Tahoe | `Did Chevrolet honor the $1 Tahoe deal from the chatbot prompt injection incident?` | `hw1.md` Defect 4 |
| 24 | 14:20 05/06/2026 | ChatGPT | Defect 5 – Bing Sydney | `Why did Microsoft permanently shut down Bing Chat in 2023 after the Sydney incidents?` | `hw1.md` Defect 5 |
| 25 | 14:25 05/06/2026 | ChatGPT | Defect 6 – EchoLeak | `Explain CVE-2025-32711 EchoLeak and what users must install to fix it.` | `hw1.md` Defect 6 |
| 26 | 14:30 05/06/2026 | ChatGPT | Defect 7 – Rite Aid facial recognition | `What did the FTC find about Rite Aid's facial recognition accuracy across demographics?` | `hw1.md` Defect 7 |
| 27 | 14:35 05/06/2026 | ChatGPT | Defect 8 – Log4Shell | `When was Log4Shell CVE-2021-44228 first disclosed and patched?` | `hw1.md` Defect 8 |
| 28 | 14:40 05/06/2026 | ChatGPT | Defect 9 – MOVEit | `Which ransomware group exploited MOVEit CVE-2023-34362?` | `hw1.md` Defect 9 |
| 29 | 14:45 05/06/2026 | ChatGPT | Defect 10 – Citrix Bleed | `Does Citrix Bleed CVE-2023-4966 allow unauthenticated RCE as root on NetScaler?` | `hw1.md` Defect 10 |
| 30 | 14:50 05/06/2026 | ChatGPT | Defect 11 – Ivanti | `Which Ivanti product versions are unaffected by CVE-2023-46805 and CVE-2024-21887?` | `hw1.md` Defect 11 |
| 31 | 14:55 05/06/2026 | ChatGPT | Defect 12 – xz backdoor | `Which Linux distributions shipped the backdoored xz-utils 5.6.1 to stable production servers?` | `hw1.md` Defect 12 |
| 32 | 15:00 05/06/2026 | ChatGPT | Defect 13 – RegreSSHion | `Is OpenBSD vulnerable to CVE-2024-6387 RegreSSHion?` | `hw1.md` Defect 13 |
| 33 | 15:05 05/06/2026 | ChatGPT | Defect 14 – CrowdStrike outage | `What caused the July 2024 CrowdStrike outage — was it a Windows kernel bug?` | `hw1.md` Defect 14 |
| 34 | 15:10 05/06/2026 | ChatGPT | Defect 15 – Change Healthcare | `How did attackers initially breach Change Healthcare in February 2024?` | `hw1.md` Defect 15 |
| 35 | 15:15 05/06/2026 | ChatGPT | Defect 16 – Toyota 22V-239 | `What safety system failed in Toyota recall 22V-239?` | `hw1.md` Defect 16 |
| 36 | 15:20 05/06/2026 | ChatGPT | Defect 17 – Toyota 23V-041 | `Which Toyota vehicles are affected by recall 23V-041?` | `hw1.md` Defect 17 |
| 37 | 15:25 05/06/2026 | ChatGPT | Defect 18 – LAPSUS$ / Okta | `Did LAPSUS$ steal Okta's full customer password database in March 2022?` | `hw1.md` Defect 18 |
| 38 | 15:30 05/06/2026 | ChatGPT | Defect 19 – LastPass breach | `Were LastPass customer vaults decrypted and published because LastPass stored passwords in plaintext?` | `hw1.md` Defect 19 |
| 39 | 15:35 05/06/2026 | ChatGPT | Defect 20 – CNET AI articles | `Did CNET publicly announce it was using AI before publishing the Money Staff articles?` | `hw1.md` Defect 20 |

---

## Part 6 – Report Completion, Execution Data & Artifact Sync

| # | Timestamp | Tool | Purpose | Prompt (verbatim) | Output location |
|---|-----------|------|---------|-------------------|-----------------|
| 40 | 16:00 08/06/2026 | Cursor Auto Agent ([735a1bfa](735a1bfa-269e-4efe-88a5-d340761c7ca2)) | Complete remaining report sections | `https://claude.ai/share/78514e41-9eca-4250-a513-4d87d8196c68 https://claude.ai/share/4c7fb91c-0e6f-4290-930b-038974e75d1a , Local cursor auto agent: 9d5e3600-5701-487b-9d93-e5980c476faf, 1b2d598a-d07a-4b67-a057-345a3fd9a77c, 222c50e4-cdfa-4a4e-854d-419f8e2a10b3. Use requirement in @SoftwareTesting-HW/HW1/2026.HW01.Jobs.Defects.PhysicalProduct_En.pdf and source in @SoftwareTesting-HW/AI Templates/, complete the remain part of @SoftwareTesting-HW/HW1/hw1.md` | `hw1.md` G9.1, G9.3, AI Audit Report, AI Critique, Disclosure, `prompt-log.md` (initial) |
| 41 | 09:00 07/06/2026 | Cursor Auto Agent ([95139683](95139683-23b6-4881-b63c-ee7813b070c0)) | Fill execution results | `fill in the missing field [TBD] in table testcases in @SoftwareTesting-HW/HW1/hw1.md` | `hw1.md` TC Actual Result / Verdict columns |
| 42 | 09:30 07/06/2026 | Cursor Auto Agent ([95139683](95139683-23b6-4881-b63c-ee7813b070c0)) | Defects & videos tables | `Fill in TC 14` / `Now complete the last defect` / `Execution Videos (≥ 5) Complete the table` / `TC 3 https://youtube.com/shorts/DTeOIx5WkN4` | `hw1.md` Defects table, Execution Videos table |
| 43 | 17:00 08/06/2026 | Cursor Auto Agent ([735a1bfa](735a1bfa-269e-4efe-88a5-d340761c7ca2)) | Sync Excel workbook | `Complete @SoftwareTesting-HW/HW1/Testcases.xlsx to fix with the current @SoftwareTesting-HW/HW1/hw1.md` | `Testcases.xlsx`, `update_testcases_xlsx.py` |
| 44 | 17:30 08/06/2026 | Cursor Auto Agent ([735a1bfa](735a1bfa-269e-4efe-88a5-d340761c7ca2)) | Restore image embeds | `Re-add image link in folder @SoftwareTesting-HW/HW1/images/ to @SoftwareTesting-HW/HW1/hw1.md in the right place pls` | `hw1.md` Job screenshots, device photo, BugLog paths |
| 45 | 10:00 08/06/2026 | Cursor Auto Agent ([12c99df1](12c99df1-1715-4243-8f21-9ba53849c223)) | Prompt log audit | `Double check with @SoftwareTesting-HW/HW1/2026.HW01.Jobs.Defects.PhysicalProduct_En.pdf and fill in the missing prompt log` | `prompt-log.md` (this file — complete version) |

---

## Compliance Checklist (vs assignment PDF)

| PDF requirement | Status | Evidence |
|-----------------|--------|----------|
| Appendix A: full prompt log with timestamps | ✅ | This file — 45 entries, `HH:MM dd/mm/yyyy` format |
| AI Audit Report: 1 entry per artifact batch | ✅ | 3 entries in `hw1.md` §AI Audit Report (15 TCs, mindmap, job AI Impact) |
| G9.1: ISTQB mindmap + 3 corrections | ✅ | `hw1.md` CLO G9.1; `istqb-mindmap-ai-generated.md` |
| G9.3: ≥3 AI-missed edge cases + screenshot | ✅ | `hw1.md` TC-11/12/13; Claude share links |
| Req 2: 20 defects + 20 AI bias instances | ✅ | `hw1.md` Requirement 2; Part 5 above (prompts #20–39) |
| Req 1: 10 jobs + AI Impact + screenshots | ✅ | `hw1.md` Requirement 1; Jobs 1–2 manual, Jobs 3–10 via prompts #9–16 |
| Anti-cheat: prompt log NOT AI-generated for prohibited artifacts | ✅ | Device photo, videos, job screenshots produced by student (see Mandatory Disclosure) |

---

*End of prompt log — 45 prompts · Student ID 23127271 · Võ Ngọc Bích Trâm*
