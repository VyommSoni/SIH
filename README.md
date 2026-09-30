<div align="center">

# 🌄 AAROHAN
### *Rise Beyond. Reach Further.*

**AI-powered scholarship & fellowship platform for Scheduled Tribe students**

![SIH 2026](https://img.shields.io/badge/SIH%202026-SIH26239-0b2545?style=for-the-badge)
![Ministry](https://img.shields.io/badge/Ministry%20of%20Tribal%20Affairs-1f6f5c?style=for-the-badge)
![Theme](https://img.shields.io/badge/Theme-Smart%20Education-1f6f5c?style=flat-square)
![Category](https://img.shields.io/badge/Category-Software-0b2545?style=flat-square)
![Status](https://img.shields.io/badge/Status-Hackathon%20Prototype-e0a030?style=flat-square)

> **Don't just process scholarship applications. Prevent application failures before submission.**

[Why](#-1-why-did-we-build-this) · [What](#-2-what-is-aarohan) · [How](#-3-how-does-it-work) · [Tech](#-4-what-is-our-tech-stack) · [Run](#-5-how-do-we-run-it) · [Team](#-6-who-is-on-the-team) · [Future](#-7-whats-next)

</div>

---

## ❓ 1. Why did we build this?

Many eligible ST students miss scholarships or lose months because of **avoidable problems**, not because they are ineligible.

| Problem | What happens |
|---|---|
| Hard to find the right scholarship | Eligible students never apply |
| Eligibility rules are unclear | Wrong applications, or students give up |
| Documents are blurry, missing, wrong or expired | Deficiency notices and delays |
| Names or dates don't match across documents | Extra rounds of checking |
| Officers check the same things by hand | Heavy workload, slow results |
| Status only says *"Processing"* | Students worry and keep asking |
| Language and low-internet barriers | Remote-area students are left out |
| Ministry can't see where the process fails | Same problems repeat every year |
| Little help after selection | Renewals and reports are missed |

These map directly to **SIH26239**: AI and document intelligence, eligibility checks, human oversight, communication, and end-to-end management after selection.

---

## 💡 2. What is AAROHAN?

A helper layer on top of the National Scholarship Portal. It does **not** replace NSP. It guides students, checks documents, and supports officers.

```mermaid
flowchart LR
    A[Discover] --> B[Understand] --> C[Prepare] --> D[Verify] --> E[Apply] --> F[Fix] --> G[Track] --> H[Succeed]
```

### 🎯 Core idea: Detect → Explain → Fix → Recheck
Most systems find problems **after** submission. AAROHAN finds them **before**: missing, blurry, wrong-type or expired documents, name or date-of-birth mismatch, incomplete form, missing signature or page.

### Who benefits

| Role | How AAROHAN helps |
|---|---|
| 👩‍🎓 **Student** | Finds the right scheme, understands the rules, fixes document issues before submitting, tracks status in their own language |
| 🧑‍💼 **Officer / Verifier** | Sees an AI case summary, extracted data, proof and confidence. Less repeated manual work |
| 🏛️ **Ministry / Admin** | Sees KPIs, bottlenecks and repeated problems. Manages scheme rules. Views the audit trail |

### ✨ Key features

| Area | Features |
|---|---|
| **Discover & Understand** | Scholarship finder with reasons, explainable eligibility, readiness score, guided application, how-to videos and FAQs |
| **Prepare & Verify** | OCR (printed, handwritten, multilingual), document classification, quality check, structured extraction, mismatch detection, **Fix My Application** |
| **Review & Track** | Officer verification queue, AI case summary, human-in-the-loop review, plain-language status timeline, notifications |
| **Access & Improve** | English and Hindi (more later), screen-reader and keyboard support, voice, low-bandwidth mode, mobile document scanning |
| **Ministry & Support** | Analytics funnel, state and district trends, process insights, grievance workflow, post-selection and renewal tracking, audit logs |
| **Saathi (Scholarship Copilot)** | RAG assistant that answers **only** from official documents, with sources |

### 🧩 Explainable eligibility (example)

Eligibility comes from **official rules stored in the database**, never from an AI guess.

| Requirement | Student's value | Result | Proof |
|---|---|---|---|
| ST category | ST | ✅ | Category certificate |
| Academic qualification | Eligible course | ✅ | Marksheet |
| Income limit | Within limit | ✅ | Income certificate |

If a rule isn't met, we say so kindly, show the requirement and the student's value, and suggest other schemes that may fit.

### 📊 Application Readiness (example: 86%)

An open estimate from five visible factors: eligibility completeness, document completeness, document quality, profile consistency, application completeness. It answers: *"If I submit now, how likely am I to face an avoidable deficiency?"* It is **not** government approval.

### 🛠️ Fix My Application (example)

- **Problem:** Income certificate could not be verified with confidence.
- **Why:** The photo is partly blurred.
- **Fix:** Retake in good light, keep the whole page in view, avoid shadows, upload a clear image or PDF.
- **Recheck:** Checks re-run automatically and the readiness score updates.

---

## 📸 Screenshots

### 📱 Student app (mobile-first)

<table>
<tr>
<td align="center" width="25%"><img src="data:image/jpeg;base64,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
