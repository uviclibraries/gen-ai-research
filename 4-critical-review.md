---
layout: default
title: 4 - Critically Review
nav_order: 6
parent: Workshop Activities
customjs: http://code.jquery.com/jquery-1.4.2.min.js
description: "Beginner’s guide to catching errors, verifying citations, and reducing bias in GenAI outputs with a simple claim-audit workflow."
last_modified_date: 2025-11-09
---
<img src="images/4-critical-review-student.png" style="float:right;width:320px;height:320px;padding:6px;" alt="Student critically reviewing a GenAI response on a laptop"> 

# Critically Review All GenAI Output for Errors

GenAI tools sometimes **hallucinate**—they state things that sound right but aren’t. This page shows you how to **spot errors quickly**, **verify claims**, and **ask for better evidence**. You’ll also learn simple prompt tweaks that reduce mistakes up front.

---

## What you’ll learn
- A 10–15 minute **Claim Audit** workflow you can run on any response.  
- How to **verify citations** (existence, relevance, quote accuracy).  
- Prompt tweaks that **lower error rates** (specificity, constraints, evidence).  
- Ways to **check and reduce bias** (gender, race, culture, time, paywalls).  

---

## Common failure modes (know these red flags)
- **No sources** or sources that don’t open.  
- **Made-up citations** (journal sounds real, article doesn’t exist).  
- **Time drift** (“as of 2022” when you asked for 2025 info).  
- **Overconfident tone** with vague numbers or superlatives (“first”, “only”).  
- **Copying training-set bias** (e.g., stereotyped images; US-centric facts).  
- **Paywall blindness** (summarizes behind-paywall material without access).

---

## Reduce errors with smarter prompts
Use **CRAFT + CE** (Context, Role, Action, Format, Target Audience + Constraints, Evidence).

**Ask for evidence on purpose**
`Return 5 numbered claims with a source link for each claim.
If you are unsure, say "NOT SURE" and stop. Do not invent sources.`


**Constrain the scope/time**

`Use sources published in 2023 or later and list the publication dates.
If a source is paywalled or inaccessible, say "PAYWALL" and skip it.`


**Request structure**
`Format: Table with columns = #, Claim, Source URL, Source Date, Confidence(0–5).`


---

## Training data bias (what it is & quick countermeasures)

Bias appears when training data is **skewed** (e.g., over-represents certain regions, genders, or professions) or **incomplete** (paywalled/under-represented fields). That can surface as narrow perspectives or stereotyped images.

<img src="images/4-white-ceos.jpeg" style="float:right;width:320px;height:320px;margin-left:10px;" alt="Illustration of three CEOs often depicted with limited demographic diversity"> 

**Counter-prompts you can use**
- **Representation:**  
  `Create an image of three CEOs with visible gender and ethnic diversity.`
- **Locale:**  
  `From a Canadian perspective, list key events around the 1814 burning of Washington during the War of 1812. Include citations.`
- **Time/quality filters:**  
  `Use 2020+ sources only; include dates and direct quotes ≤10 words with line refs if available.`

---

## The Claim Audit (10–15 min)

**Step 1 — Extract claims from the model**
`From the answer above, extract 5–8 key claims.
For each claim, provide: Claim (≤20 words), Source URL, Source Title, Source Date.
If a claim lacks a source, mark "NO SOURCE".`


**Step 2 — Verify independently**
Open each source yourself. Check that:
- The **page exists** and actually matches the claim.  
- The **quote or fact** is present and not distorted.  
- The **date** is appropriate for your question (recent enough).  


**Step 3 — Log the results (use this table)**
| # | Claim | Source URL | Source Date | Check Result (✅/❌) | Notes / Exact Quote |
|---|-------|------------|-------------|----------------------|---------------------|
| 1 |       |            |             |                      |                     |
| 2 |       |            |             |                      |                     |



**Step 4 — Ask the model to correct itself**

`Based on my verification notes below, correct any inaccurate or unsupported claims.
If evidence is missing, replace the claim with "NOT VERIFIED" or remove it.
Keep only what is supported; list corrected claims with sources and dates.`


**Step 5 — (Optional) Teach-back summary**

`Produce a 120-word summary using only the verified claims.
Include 2 short quotes (≤10 words) with citation labels [S1], [S2].`


---

## Extra checks for citations & quotes

- **Exists?** The article/book/site is real and accessible.  
- **Matches?** The text actually says what the model claims.  
- **Quote hygiene:** Quotes are short (≤10 words) and appear verbatim.  
- **Dates:** Recent enough for your task; date is shown.  
- **Paywalls:** If paywalled, the model should admit it (don’t trust invented summaries).  
- **Bias sweep:** Ask for a diverse or local perspective where relevant.

---

## Practice (15–20 min)

1) **Topic you know well**  
Ask a question about a local person/place/topic you can verify from your own knowledge or trusted sites.  
**Prompt:**
`Return 6 numbered claims with a source URL and date for each claim.
If unsure, say "NOT SURE". Do not invent sources.
Format: table with #, Claim, Source, Date.'

Run the **Claim Audit** steps. Note any ❌ and correct them.

2) **Bias & perspective**  
Re-ask the same question with diversity or locale constraints (e.g., “Canadian perspective”, “gender-diverse examples”). Compare outputs.

3) **Image bias spot-check (optional)**  
Generate an image (if your tool supports it). Check for artifacts (extra fingers, garbled text) and demographic stereotypes. Adjust the prompt to improve representation and realism.

> **Badge evidence:** Save a screenshot of your **Evidence Table** with at least one ❌ correction, or a before/after bias-adjusted output.

---

## Reflection (2–3 min)
- Which red flag showed up most (no source, wrong date, vague numbers)?  
- What prompt change made the biggest quality jump (constraints, evidence, format)?  
- How will you bake the Claim Audit into your weekly workflow?

---

## Quick reference prompts (copy/paste)

**Evidence demand**
List 5 numbered claims with a working source link and publication date for each.
If you can’t find a source, say "NO SOURCE" for that claim.


**Time filter**
Use sources from 2023+ only. Show dates next to each citation.


**Non-invention rule**
If unsure or the source is paywalled, say "NOT SURE" or "PAYWALL"—do not guess.


---

Critical Review: add claim-audit workflow, evidence/correction templates, bias counter-prompts; fix typos, alt text, and link hygiene

[NEXT STEP: Privacy & The Environment](5-privacy.html){: .btn .btn-blue }

