---
layout: default
title: Intermideate - Prompt Design
nav_order: 3
parent: Workshop Activities
customjs: http://code.jquery.com/jquery-1.4.2.min.js
description: "Intermediate prompt design: reusable patterns, chaining, tone, scope, examples, and structured outputs—with quick practices."
last_modified_date: 2025-11-09
--- 

# Prompt Design — Intermediate
<img src="images/prompt-design-image.png" style="float:right;width:320px;padding:6px;" alt="Student working on intermediate GenAI prompt design">
If you get stuck during this in-class exercise, ask the instructor. Let’s level up.

---

## What you’ll learn
- A quick **CRAFT** refresh and how to extend it with constraints/evidence.
- **Reusable prompt patterns** (Summarizer, Explainer, Tutor, Planner, Critic, Formatter).
- **Prompt chaining** to refine results and build on previous steps.
- How to **control tone, scope, and structure** so outputs are auditably useful.
- How to spot/avoid common failure modes (vagueness, missing evidence, scope creep).

> **Privacy note:** Don’t paste confidential or personal data. Redact names/emails/IDs (e.g., `[Researcher_A]`, `[Email_1]`).
---

## CRAFT (fast refresh)
Use **CRAFT** and add constraints/evidence when facts matter.

- **Context** — why you’re asking; **Role** — who to act as; **Action** — exact deliverable;  
  **Format** — headings/bullets/JSON; **Target Audience** — who it’s for.
- **Constraints** (word/time limits, must include/avoid) and **Evidence** (citations/URLs).

> Typo fix from earlier pages: “Target Audience,” not “Targe Audience.” Accuracy starts with you.

**Plus:**
- **Constraints**: limits + must include/avoid (reduces errors + fluff)
- **Evidence**: citations/URLs when facts matter
- **Acceptance Criteria** (the “definition of done”): what a correct answer must include
---

## Patterns library (copy/paste)
Use these as building blocks; swap in your topic.

### 1) Summarizer 
**Prompt**
- Context: `You are summarizing for a reader who needs only what is supported by the text.`
- Role: `Academic editor`
- Action: `Summarize the text into 140–170 words.`
- Format: `Headings: Key claim | Evidence used | Limitations | What is NOT stated`
- Constraints: `No new facts. If missing, say “NOT PROVIDED.”`
- Evidence: `Include 2 citations or quotes (<=10 words each).`

### 2) Explainer 
**Prompt**
- Role: `Subject expert`
- Action: `Explain <concept> for <audience>.`
- Format: `5 bullets: Definition | Why it matters | Core idea | Simple example | Common mistake`
- Constraints: `Plain language; avoid jargon; <=120 words.`

### 3) Planner 
**Prompt**
- Role: `Project planner`
- Action: `Produce a 5-step plan to achieve <goal>.`
- Format: `Table: Step | Objective | Inputs | Deliverable | Acceptance criteria`
- Constraints: `No step longer than 2 lines.`

### 4) Critic 
**Prompt**
- Role: `Critical reviewer`
- Action: `Assess my draft for Accuracy, Coverage, Clarity, Evidence, and Formatting.`
- Format: `Table: Category | Score(1–5) | Evidence from text | Fix`
- Constraints: `Do not rewrite yet. Only diagnose.`

### 5) Formatter 
**Prompt**
- Role: `Technical formatter`
- Action: `Reformat this into Markdown with H2/H3 and numbered steps.`
- Constraints: `Do not change meaning. Flag missing refs as [MISSING REF].`

### 6) Template pattern (placeholders)
**Prompt**
`Use this exact template. Do not add extra sections:
Title:
Goal (1 sentence):
Key points (3 bullets):
Risks/uncertainties (2 bullets):
Next actions (3 numbered steps):`
---

## Prompting (the “3-step upgrade”)
Chaining beats one giant prompt. You get less chaos and more control.

**Chain format:**
1) **Draft** the output  
2) **Critique** it using acceptance criteria  
3) **Revise** based on critique

**Example chain (copy/paste)**  
**Step 1: Draft**
`Create a structured answer on <topic>. Format: 6 bullets with headings. Include 2 sources.`

**Step 2: Critique**
`Check your answer against these acceptance criteria:
- Has a clear definition (1 sentence)
- Has 2 verifiable sources (URLs)
- No claims without evidence
- Max 120 words
Return a table: Criterion | Pass/Fail | Fix`

**Step 3: Revise**
`Rewrite the answer applying all fixes. If you cannot verify a claim, mark it “NOT SURE.”`

---

## Advanced tips & examples

1) **Start a new chat when context changes**
<br><img src="images/1-new-topic.png" style="width:400px;" alt="Copilot’s New Topic button">
- Old context can contaminate answers. Use **New Topic** (or “new chat”) for unrelated tasks.

2) **Tone control**
- Poor: `Weather in Paris.`
- Better: `Give me a lighthearted weather update for Paris, France, with a humorous twist.`
- Now try: same request in *neutral* and *formal* tones. Which suits your goal?

3) **Examples & analogies (few-shot prompting)**
- Poor: `Explain cyclones.`
- Better: `Explain how cyclones form, using Cyclone Nisarga as the example. Provide sources.`
- Try adding one mini example of your own to guide the style.

4) **Limit scope**
- Poor: `Tell me everything about weather.`
- Better: `Outline 4 factors that influence thunderstorm formation; 1 sentence each; list sources.`
- Scope: `fewer errors, faster checking.`

5) **Iterate with acceptance criteria**
- Initial: `Weather in London.`
- Refined: `Weekend forecast for London, UK, with any weather warnings. Format: bullets; include source links.`
- Add **acceptance criteria**: “Contains date range, temperature range, precipitation chance; max 80 words.”

6) **Prompt chaining (build on prior output)**
- First: `What factors affect local weather conditions?`
- Then: `Considering those factors, draft a 3-bullet safety advisory for hikers near San Francisco this weekend. Include sources.`
- Chaining = focused refinement, not rambling.

7) **Leverage precedents (transfer learning)**
<img src="images/1-weather-student.jpeg" style="width:320px;height:320px;" alt="AI-generated student learning about weather">
- Prior prompt: `Explain El Niño and its impact on global weather patterns.`
- New prompt: `Explain La Niña and its impact on global weather patterns. Provide sources.`

8) **Assign a useful role**
- Role: `You are the head of a creative department at an ad agency.`
- Action: `Brainstorm 5 campaign taglines for <product>.`
- Constraints: `Family-friendly; avoid superlatives; 6 words max per tagline.`

9) **Image generation (availability varies by tool/tier)**
- Try **[Meta.ai](https://meta.ai){:target="_blank" rel="noopener"}** or **[Copilot](https://copilot.microsoft.com){:target="_blank" rel="noopener"}**.
- Prompt: `Create an image of a Grade 2 student learning about the weather in a classroom.`  
- Constraints: `Check for artifacts (extra fingers, text gibberish, anatomy errors) before using.`

> **Badge evidence:** capture a screenshot of your own image prompt + output.

---

## Practice set (15–20 min)

**A. Global warming (text)**
- Initial: `What is global warming and what are its causes? Provide sources.`
- Scope: `Limit to 300 words at a Grade 4 reading level.`
- Tone (style shift): `Reword in a playful style suitable for Grade 4, while keeping facts accurate and cited.`

(Avoid asking for an identifiable author’s proprietary style; keep it generic.)

**B. Global warming (image)**
- Prompt: `Create an image of a Grade 4 student learning about global warming in a classroom.`
<img src="images/1-global-warming-seuss.jpeg" style="width:320px;height:320px;" alt="AI-generated drawing of a student learning about global warming">
- Variation: `Adjust the illustration to look like simple children’s book line art.`

**C. Lesson plan chaining**
- Start a new chat, then: `I teach Grade 4. Generate a 60-minute lesson on local weather with a 30-minute hands-on activity.`
- Format: `Objectives, Materials, Steps with times, Assessment, Differentiation.`
- Follow-up: `Provide step-by-step student instructions for the activity at a Grade 4 reading level.`
- Add acceptance criteria: `The plan must fit 60 minutes total, list 3 materials only, and include one formative check.`

**Reflection (2–3 min)**
- Which acceptance criteria improved quality the most?  
- Where did tone or scope reduce errors?  
- What will you reuse as a personal template?

---

## Self-check (2 min)
- Did you specify **CRAFT + constraints/evidence**?
- Is tone and **scope** appropriate for your audience?
- Did you **chain** prompts rather than rewrite from scratch?
- Are sources **verifiable** (and not just names without links)?
- Would your output pass your own **acceptance criteria**?

---
### Acceptance criteria mini-library
- **Summary**: 120–150 words, neutral tone, no new facts, 1 quote ≤10 words.
- **Plan**: 5 steps; each has Objective • Inputs • Acceptance; total ≤180 words.
- **Table**: Columns fixed; max 6 rows; no empty cells.
- **Evidence**: Each claim has URL + date; if unsure → “NOT SURE”.


## Go further
A practical overview of techniques worth skimming next:  
[Prompt engineering techniques](https://www.geeky-gadgets.com/prompt-engineering-techniques/){:target="_blank" rel="noopener"}

[NEXT STEP: Idea Generation](3-idea-generation.html){: .btn .btn-blue }




