<!--
---
layout: default
title: 7 - Literature Review Tools
nav_order: 9
parent: Workshop Activities
customjs: http://code.jquery.com/jquery-1.4.2.min.js
description: "A simple scope→search→skim→synthesize workflow with safe GenAI assists, note-taking templates, and citation hygiene."
last_modified_date: 2025-11-09
---
-->

# Literature Review Tools

If you’re new to AI-assisted lit reviews, start here:
## [AI: Tools for Literature Reviews (Introduction)](https://uviclibraries.github.io/ai-lit-reviews-intro/workshop-activities.html){:target="_blank" rel="noopener"}

---

## What you’ll learn
- A **four-step workflow**: scope → search → skim → synthesize.  
- How GenAI can **suggest queries** and **structure notes** (without fabricating citations).  
- A **triage table** for quick include/maybe/exclude decisions.  
- A **synthesis matrix** you can paste into your notes or a spreadsheet.  
- **Citation hygiene** (DOIs, dates, paywalls, and avoiding fake references).

> Ground rule: GenAI can brainstorm queries and structure notes. **Do not** accept citations the model invents. Always verify authors, titles, venues, DOIs/URLs, and dates yourself.

---

## Before you start
- Have your **question** in one sentence.  
- Open your **library search** (UVic discovery), **Google Scholar**, and your preferred tool (Perplexity, Copilot, ChatGPT, Gemini, Claude—any is fine).  
- Use a **reference manager** (Zotero or equivalent) ready to capture PDFs/DOIs.

---

## Step 1 — Scope your question (2–5 min)

Pick a simple framing (use one):

- **PICo** (Population • Interest • Context)  
- **SPIDER** (Sample • Phenomenon • Design • Evaluation • Research type)

**Prompt (copy/paste):**
```

Role: research methods tutor
Action: Turn my topic into PICo and SPIDER framings; list synonyms for each element.
Topic: <paste your one-sentence question>
Format: Table with Columns = Element, My term, 5–8 synonyms/alternates.
Constraints: No citations; just terms I can test in databases.

```
---

## Step 2 — Search (5–10 min)

Use the terms to build real queries in UVic discovery, subject databases, and Google Scholar. Let GenAI help **draft** the strings—then you run them.

**Prompt:**
```

Action: Propose 3 Boolean search strings for databases and 2 for Google Scholar.
Input terms: <paste your PICo/SPIDER terms>
Constraints: Include truncation and phrase quotes where sensible.
Return: Code blocks only; do not invent or cite papers.

```

Run the queries yourself. **Open actual results**, export RIS/DOIs to your manager.

---

## Step 3 — Skim & triage (10–15 min)

Skim titles/abstracts. Use this **triage table** (paste into notes/Sheets/Notion):

**Triage (blank)**
| Decision | Reason (≤10 words) | Title | First Author | Year | Venue/DOI |
|---|---|---|---|---|---|
| Include/Maybe/Exclude |  |  |  |  |  |

Aim for 8–15 “Include/Maybe” items before moving on.

---

## Step 4 — Synthesize (15–20 min)

For each included paper, capture concise, comparable notes.

**Synthesis matrix (blank)**
| Paper (APA short) | Question/Goal | Method & Sample | Key Findings | Limits | Use in my review |
|---|---|---|---|---|---|

**Prompt (per paper, optional):**
```

Role: careful note-taker
Action: Produce a structured abstract from the excerpt below.
Format: Question/Goal; Method & Sample; Key Findings; Limits; 2 short quotations (≤10 words) with page/section refs if present.
Constraints: Use only the pasted text; do not invent citations or page numbers; if missing, write [NOT IN EXCERPT].

```

Paste the **actual abstract** or a short excerpt from the **PDF you opened**, not just a URL.

---

## Safer GenAI usage (what to ask vs what to avoid)

**Good asks**
- Suggest synonyms and Boolean strings.  
- Outline headings for a related-work section.  
- Normalize your notes into a consistent table.  
- Draft inclusion/exclusion **criteria** (you approve them).

**Avoid**
- Accepting generated **citations** you haven’t verified.  
- Summaries of **paywalled** papers the tool cannot access.  
- Claims without **publication venue** and **year**.

---

## Copy-paste prompt kit

**Inclusion/exclusion criteria**
```

Action: Propose inclusion and exclusion criteria for my review.
Context: <2–3 lines about scope and audience>
Format: Two lists (bullets); keep each item ≤12 words.

```
**Query refinement**
```
Action: Given these results (paste 3 titles/abstract snippets), suggest 2 narrower and 2 broader search strings.
Constraints: Boolean-ready; no fake paper names; code blocks only.

```
**Outline builder**
```
Role: academic editor
Action: Draft an outline for a 1200-word related work section based on my included papers (list below).
Format: H2/H3 headings; notes under each with which paper supports it (Author-Year).
Constraints: Use only my list; no new sources.

```
---

## Hands-on (15–25 min)

1) Run Step 1 & 2 with your topic; capture **3–5** promising papers.  
2) Fill the **Triage** table for those papers.  
3) Complete **Synthesis** rows for **2** papers using real text.  
4) Build a short **outline** with which paper supports each point.

> **Badge evidence:** screenshot of your triage table and a synthesis matrix row.

---

## Citation hygiene (2–3 min)

- Record **author, year, title, venue, DOI/URL** for every included paper.  
- Prefer the **publisher DOI** over blog mirrors.  
- For quotes, record **page/section**.  
- If a tool proposes a citation, **assume it’s wrong** until you verify.

---

## Quick tool map (use what you have)

- **Search/Discovery:** UVic library search, subject databases, Google Scholar.  
- **Query help & notes:** Perplexity, Copilot, ChatGPT, Gemini, Claude (for **queries/structure**, not citations).  
- **Citation managers:** Zotero (recommended), Mendeley, EndNote.  
- **Graph/discovery aids (optional):** ResearchRabbit, Connected Papers (always verify).

---
`Lit Review: add scope→search→skim→synthesize workflow, prompts, triage/synthesis tables, and citation hygiene`

## PRISMA-lite log (keep it simple)
| Stage | Count | Notes |
|---|---|---|
| Records identified |  |
| Duplicates removed |  |
| Screened (title/abstract) |  |
| Full-text assessed |  |
| Included in review |  |

> Tip: keep this in your notes or a sheet; it saves time later.


[NEXT STEP: Earn a Workshop Badge](informal-credentials.html){: .btn .btn-blue }
```
