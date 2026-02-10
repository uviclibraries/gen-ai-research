---
layout: default
title: 1 - Prompt Design 1
nav_order: 3
parent: Workshop Activities
customjs: http://code.jquery.com/jquery-1.4.2.min.js
description: "Beginner-friendly prompt design with the CRAFT framework, quick-start templates, and step-by-step practice."
last_modified_date: 2025-11-09
--- 

# Prompt Design Introduction
<img src="images/prompt-design-image.png" style="float:right;width:320px;padding:6px;" alt="Student at a computer learning effective GenAI prompt design">

**Estimated time:** 20–30 minutes  
If you get stuck, ask the instructor. Have fun—this is hands-on.

---

## What you’ll learn
- A simple framework (**CRAFT**) for writing prompts that produce clearer, more useful results.  
- How to turn a weak, vague prompt into a strong one with structure and constraints.  
- How to evaluate responses for accuracy and fit to your goal.

## Before you start
Open **one** tool in your browser:
- [Perplexity](https://www.perplexity.ai/){:target="_blank" rel="noopener"} (often works without an account) **or** [Microsoft Copilot](https://copilot.microsoft.com/){:target="_blank" rel="noopener"} (UVic-licensed option available).  
You may use other tools if you prefer:
[ChatGPT](https://chat.openai.com/){:target="_blank" rel="noopener"},
[Meta.ai](https://www.meta.ai/){:target="_blank" rel="noopener"},
[Claude](https://claude.ai/){:target="_blank" rel="noopener"},
[Google Gemini](https://gemini.google.com/){:target="_blank" rel="noopener"}.

> **Privacy note:** Don’t paste confidential or personal data. Redact names/emails/IDs (e.g., `[Researcher_A]`, `[Email_1]`). For data-handling details, see the UVic guidance linked on the Pre-Workshop page.

---

## Prompt Design Basics: The CRAFT Framework
Getting started is easy; getting **good** takes structure and practice. Use **CRAFT**:

- **Context** — Background and purpose. Who’s asking and why?  
  _Example:_ `I’m preparing a 60-minute lesson about weather for Grade 2.`

- **Role** — Who should the assistant act as?  
  _Example:_ `Act as an elementary school teacher.`

- **Action** — What exactly should be produced?  
  _Example:_ `Create a one-hour lesson plan plus a 30-minute activity.`

- **Format** — How should it be structured?  
  _Example:_ `Return bullet points with headings: Objectives, Materials, Steps, Assessment.`

- **Target Audience** — Who is this for? Adjust tone and level.  
  _Example:_ `Write at a Grade 2 reading level.`

> **CRAFT+ (recommended):** Add **Constraints** (time, word count, must include/avoid), and **Evidence** (citations/URLs) when facts matter.

---

## Bad → Better → Best (weather lesson)

**Bad (too vague)**
`Tell me about the weather.`

_Why it fails:_ No audience, no goal, no format. You’ll get generic fluff.

**Better (uses CRAFT)**
Context: `I’m teaching a one-hour lesson about weather.`
Role: `Elementary school teacher.`
Action: `Create a lesson plan with a 30-minute activity.`
Format: `Bullet points with headings: Objectives, Materials, Steps, Assessment.`
Target Audience: `Grade 2 students.`


**Best (CRAFT+)**
Context: `I’m teaching a one-hour weather lesson next week.`
Role: `Elementary school teacher.`
Action: `Create a timed lesson plan plus a 30-minute activity that reinforces key ideas.`
Format: `Bullet points with headings: Objectives, Materials, Steps (with times), Assessment, Differentiation.`
Target Audience: `Grade 2 students.`
Constraints: `Use simple language; avoid jargon; total plan <= 200 words; activity must require minimal materials.`
Evidence: `Provide 2 age-appropriate sources or curriculum references with URLs.`


---

## Let’s practice!

### 1) Test a poor prompt (2 min)
Copy/paste into your tool:

`Tell me about the weather.`

<img src="images/prompt-lesson-poor.png" alt="Copilot showing a generic response to a vague weather prompt"><br>
**Question:** What’s missing? (Audience, goal, format, constraints, evidence.)

### 2) Try the improved prompt (5–7 min)
Copy/paste this:

`Context: I’m teaching a one-hour lesson about weather.
Role: Elementary school teacher.
Action: Create a lesson plan with a 30-minute activity.
Format: Bullet points with headings: Objectives, Materials, Steps, Assessment.
Target Audience: Grade 2 students.
Constraints: Keep it concise; activity uses common classroom supplies.
Evidence: Include 2 sources or curriculum references with URLs.`

<img src="images/1-prompt-weather-lesson.png" alt="Copilot producing a structured Grade 2 weather lesson plan"><br>

**Discuss:**
- How is this response better than the vague prompt?  
- Do you have the **weather expertise** to check the facts?  
- Do you have the **teaching expertise** to judge if the plan is realistic for Grade 2?

> _Every time we use GenAI tools we must ask: **Do I have the expertise to evaluate this?** If not, verify with trusted sources or a domain expert._

### 3) Your domain (8–10 min)
Pick one or two topics you know well (e.g., “What are the origins of skateboarding?”).

- Ask your tool one focused question about Topic A.  
- Is the answer accurate? What evidence is shown?  
- Use a follow-up prompt to improve accuracy or clarity.  
- Ask a question about Topic B and compare.  
- Did you have to look up sources to verify claims?

> **Badge evidence:** Capture a screenshot of one “topic you know well” prompt and output (required for the workshop badge).

---

## Self-check (2 min)
- Did you include **all five CRAFT elements**?  
- Did you add **constraints** and request **evidence** if facts matter?  
- Is the response **structured** the way you asked?  
- Did you **verify** at least one claim with an independent source?

---

## Go further
Want more patterns and examples? This overview of practical techniques is a nice next read:  
[Prompt engineering techniques](https://www.geeky-gadgets.com/prompt-engineering-techniques/){:target="_blank" rel="noopener"}


[NEXT STEP: Intermediate Prompt Design](2-prompt-inter.html){: .btn .btn-blue }
