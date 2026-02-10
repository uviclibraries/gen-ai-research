---
layout: default
title: 3 - Idea Generation
nav_order: 5
parent: Workshop Activities
customjs: http://code.jquery.com/jquery-1.4.2.min.js
description: "Beginner-friendly idea generation with a simple diverge→cluster→converge workflow, measurable criteria, and safe summarization."
last_modified_date: 2025-11-09
--- 

# Idea Generation — Introduction
<img src="images/prompt-design-image.png" style="float:right;width:320px;padding:6px;" alt="Student at a computer brainstorming with GenAI">
If you get stuck as you work through this in-class exercise, ask the instructor. Have fun—this one is hands-on.

---

## Reminder on academic integrity
You **must have permission** from your instructor to use GenAI in any assessed work. Some courses forbid it; others allow limited or full use. Follow your course outline and citation rules. Using GenAI without permission is academic misconduct under UVic’s [Academic Integrity Policy](https://www.uvic.ca/students/academics/academic-integrity/index.php){:target="_blank" rel="noopener"}.

---

## What you’ll learn
- A simple, repeatable ideation pipeline: **diverge → cluster → converge**.  
- How to turn topics into **measurable research questions**.  
- How to **summarize safely** (tool limits, chunking, verification).

## Before you start
Open one tool: Copilot, Gemini, ChatGPT, Perplexity, or Claude (any is fine).  
> **Safety:** Don’t paste confidential/personal data. Redact names/emails/IDs (e.g., `[Researcher_A]`, `[Email_1]`).

---

## A. Diverge (5–7 min): create many options
**Goal**: generate a broad list of plausible directions without judging them yet.

**Prompt (copy/paste, replace angle brackets):**
`**Role**: Research mentor.`
`**Action**: Propose 20 distinct topic ideas about <your broad area>.`
`**Format**: Table with columns = Idea, One-sentence rationale, Tags(3).`
`**Constraints**: No duplicates; vary methods (survey, experiment, case study), contexts (K–12/higher ed/industry), and scales (classroom/institution/community).`


**Now try your own:** If 20 is too many, ask for 10. If it’s too generic, add constraints (e.g., “Canada only,” “undergraduate makerspaces,” “low-cost data”).

---

## B. Cluster (5–7 min): find patterns
**Goal**: reduce noise by grouping related ideas.

**Prompt:**
- `**Action**: Cluster the 20 ideas into 5 labeled themes.`
- `**Format**: Table with columns = Theme, Ideas included, Why this theme matters (≤20 words).`
- `**Constraints**: No theme overlaps; each idea appears once.`


Optional follow-up:
- `**Action**: For each theme, generate 2 “stretch” variations that increase novelty without losing feasibility.`


---

## C. Converge (8–10 min): pick winners with criteria
**Goal**: select 2–3 ideas worth pursuing using measurable criteria.

**Prompt:**
- `**Action**: Score each theme 0–5 on Novelty, Feasibility (skills/time), Data availability, Scope fit, Potential impact.`
- `**Format**: Table with columns = Theme, Novelty, Feasibility, Data, Scope, Impact, Notes.`
- `**Constraints**: Brief notes with concrete risks or assumptions.``

**Decide:** Keep the top 2–3 themes. Write 1–2 risks you will check next (e.g., “access to participants,” “IRB/ethics needed,” “data exists?”).

---

## D. Turn topics into measurable research questions (RQ drill)
**Goal**: convert a theme into sharp questions you can test/evaluate.

**Prompt:**

- `**Role**: Research methods tutor.`
- `**Action**: Propose 5 research questions for the theme <chosen theme>.`
- `**Format**: Table with columns = RQ, Variables/constructs, Method (1 line), Measurable outcome, Feasibility note.`
- `**Constraints**: Use clear, observable outcomes; avoid vague verbs; align with an undergraduate project scope.`

**Refine one RQ** with acceptance criteria:
- `**Action**: Rewrite RQ #2 so it is specific and measurable.`
- `**Constraints**: Time-bounded; identifies population and setting; feasible data source; ethical to implement.`


---

## E. Summarize a document safely (tool limits & chunking)
Free tiers and some enterprise tools limit input size. If a tool can’t “read” the whole article, it should say so. Ask it to be explicit—and chunk long text.

1) **Pick an article** (example news story):  
[LEGO helps Langford man recapture life after induced coma in 2018](https://www.saanichnews.com/local-news/lego-helps-langford-man-recapture-life-after-induced-coma-in-2018-7333837){:target="_blank" rel="noopener"}

2) **Ask the tool to confirm capacity first:**

`Can you summarize the article at this URL? If not, say "TOO LONG" and ask me to paste text in chunks of your preferred size.
URL: https://www.saanichnews.com/local-news/lego-helps-langford-man-recapture-life-after-induced-coma-in-2018-7333837`


3) **If too long, paste in chunks:**  
`Here is CHUNK 1/3 (do not summarize yet). Acknowledge receipt only.`

(Repeat for CHUNK 2/3 and 3/3.)

4) **Then summarize across chunks:**
`Action: Produce a 5-bullet summary using only the content from CHUNKS 1–3.
Constraints: No new facts; quote 2 short phrases (≤10 words) with bullet numbers.`


5) **Compare summaries:** `Are the “quick” and “expanded” versions different in quality/coverage?`

---

## Guided examples you can try right now

**1) Topic exploration (makerspaces)**

`I am an undergraduate student starting an honours project about university makerspaces.
Generate 15 distinct topics. Vary method (survey/experiment/case), context (course/program/library), and outcome (learning/employability/access).
Return a table with Idea, Rationale, Tags.`

Now try a topic you care about.

**2) Research questions from a bullet**
`Suggest 5 research questions with measurable outcomes for:
"Evaluate the effectiveness of makerspace programs."
Return a table with Research Questions, Variables, Method, Outcome, Feasibility note.`

Then run the **Research Questions drill** above to tighten one question.

**3) Article summary (with limits)**
- Ask for capacity, then either summarize the URL or paste chunks.  
- Follow with: `Expand to ≥5 bullets; keep quotes short; no new facts.`

> **Note:** Limits change over time. If a tool doesn’t acknowledge limits, assume it may not have processed everything—ask it to show its work.

---

## Reflection (2–3 min)
- Which **two criteria** mattered most for your down-selection?  
- Which **prompt change** improved quality the most—tone, scope, or format?  
- What **risk** will you check next (data, ethics, access)?

> **Badge evidence:** Save a screenshot of your “top 3” table (with scores) or your “5 research questions” table.

---

## Self-check (2 min)
- Did you **diverge** (≥10 ideas), **cluster** (clear themes), and **converge** (scored & selected)?  
- Are your Research Questions **measurable** and scoped to your time/resources?  
- Did you verify at least one claim or data assumption?

---

## Go further
For more prompting techniques (tone, examples, format control), a short overview you can skim next:  
[Prompt engineering techniques](https://www.geeky-gadgets.com/prompt-engineering-techniques/){:target="_blank" rel="noopener"}


[NEXT STEP: Critical Review](4-critical-review.html){: .btn .btn-blue }
