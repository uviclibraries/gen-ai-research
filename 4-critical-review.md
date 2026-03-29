---
layout: default
title: 4 - Critically Review
nav_order: 5
parent: Workshop Activities
---

# Critically Review All GenAI Output for Errors

![Student critically reviewing a GenAI response on a laptop](images/4-critical-review-student.png)

GenAI tools sometimes **hallucinate**—they state things that sound right but aren't. This page teaches you a general-purpose methodology for spotting errors, verifying claims, and asking for better evidence. You'll also learn prompt tweaks that reduce mistakes up front.

> **Note:** The skills on this page apply to any GenAI tool and any task. If you are specifically evaluating AI-powered **literature search tools** (Research Rabbit, Elicit, Consensus, etc.), the **[Literature Searching with AI](https://lib.uvic.ca/ai-lit-search)** workshop applies this same critical lens to that context.

---

## What you'll learn

* A 10–15 minute **Claim Audit** workflow you can run on any GenAI response.
* How to **verify citations** (existence, relevance, quote accuracy).
* Prompt tweaks that **lower error rates** (specificity, constraints, evidence requests).
* Ways to **check and reduce bias** (gender, race, culture, time, paywalls).

---

## When you MUST audit (don't skip this)

Audit GenAI outputs when:

* You will **publish or share** the output (slides, assignments, reports).
* The answer includes **numbers, dates, "first/only/best" claims**, or legal/medical advice.
* The output will influence decisions (policy, grading, procurement, research claims).

---

## Common failure modes (know these red flags)

* **No sources** or sources that don't open.
* **Made-up citations** (journal sounds real, article doesn't exist).
* **Time drift** ("as of 2022" when you asked for 2025 info).
* **Overconfident tone** with vague numbers or superlatives ("first", "only").
* **Copying training-set bias** (e.g., stereotyped images; US-centric facts).
* **Paywall blindness** (summarizes behind-paywall material without access).

---

## Reduce errors with smarter prompts

Use **CRAFT + CE** (Context, Role, Action, Format, Target Audience + Constraints, Evidence).

### Evidence demand (copy/paste)
```
Return 6 numbered claims. For each claim: Source URL + source date.
If you can't find a source, write "NO SOURCE" for that claim.
Do not invent citations.
```

### Structure request (copy/paste)
```
Format: Table with columns = #, Claim (<=20 words), Source URL, Source Date, Confidence (0–5).
```

### Time filter + paywall rule (copy/paste)
```
Use sources published in 2023 or later and show dates.
If a source is paywalled or inaccessible, write "PAYWALL" and skip it.
```

---

## Training data bias (what it is & quick countermeasures)

Bias appears when training data is **skewed** (e.g., over-represents certain regions, genders, or professions) or **incomplete** (paywalled or under-represented fields). That can surface as narrow perspectives or stereotyped images.

![Illustration of three CEOs often depicted with limited demographic diversity](images/4-white-ceos.jpeg)

**Counter-prompts you can use:**

* **Locale constraint:**
  `Answer from a Canadian context. If norms differ by country, label them explicitly. Include Canadian sources where possible.`

* **Representation constraint:**
  `Give examples that include gender and cultural diversity. Avoid stereotypes.`

* **Perspective sweep:**
  `Provide 3 perspectives: mainstream, critical, and Indigenous/local community (where relevant). Cite sources for each.`

---

## The Claim Audit workflow (10–15 min)

**Step 1 — Extract claims from the model**
```
From the answer above, extract 5–8 key claims. For each claim, provide:
Claim (≤20 words), Source URL, Source Title, Source Date.
If a claim lacks a source, mark "NO SOURCE".
```

**Step 2 — Verify independently**

Open each source yourself. Check that:
* The **page exists** and actually matches the claim.
* The **quote or fact** is present and not distorted.
* The **date** is appropriate for your question (recent enough).

**Step 3 — Log your results**

For each claim record:
* Claim
* Source URL
* Source Date
* Check Result (✅ / ❌)
* Notes / Exact Quote

**Step 4 — Ask the model to correct itself**
```
Based on my verification notes below, correct any inaccurate or unsupported claims.
If evidence is missing, replace the claim with "NOT VERIFIED" or remove it.
Keep only what is supported; list corrected claims with sources and dates.
```

**Step 5 — (Optional) Teach-back summary**
```
Produce a 120-word summary using only the verified claims.
Include 2 short quotes (≤10 words) with citation labels [S1], [S2].
```

---

## Extra checks for citations & quotes

* **Exists?** The article/book/site is real and accessible.
* **Matches?** The text actually says what the model claims.
* **Quote hygiene:** Quotes are short (≤10 words) and appear verbatim.
* **Dates:** Recent enough for your task; date is shown.
* **Paywalls:** If paywalled, the model should admit it — don't trust invented summaries.
* **Bias sweep:** Ask for a diverse or local perspective where relevant.

---

## Practice (15–20 min)

**1) Topic you know well**

Ask a question about a local person, place, or topic you can verify from your own knowledge or trusted sites.

**Prompt:**
```
Return 6 numbered claims with a source URL and date for each.
If unsure, say "NOT SURE". Do not invent sources.
Format: table with #, Claim, Source, Date.
```

Run the Claim Audit steps above. Note any ❌ and correct them.

**2) Bias & perspective**

Re-ask the same question with diversity or locale constraints (e.g., "Canadian perspective", "gender-diverse examples"). Compare the two outputs.

**3) Image bias spot-check (optional)**

Generate an image if your tool supports it. Check for artifacts (extra fingers, garbled text) and demographic stereotypes. Adjust the prompt to improve representation and realism.

> **Badge evidence:** Save a screenshot of your Evidence Table with at least one ❌ correction, or a before/after bias-adjusted output.

---

## Reflection (2–3 min)

* Which red flag showed up most (no source, wrong date, vague numbers)?
* What prompt change made the biggest quality jump (constraints, evidence, format)?
* How will you build the Claim Audit into your regular workflow?

---

## Quick reference prompts (copy/paste)

**Evidence demand**
```
List 5 numbered claims with a working source link and publication date for each.
If you can't find a source, say "NO SOURCE" for that claim.
```

**Time filter**
```
Use sources from 2023+ only. Show dates next to each citation.
```

**Non-invention rule**
```
If unsure or the source is paywalled, say "NOT SURE" or "PAYWALL" — do not guess.
```

---

[NEXT STEP: Privacy & Data Safety](5-privacy.html)
