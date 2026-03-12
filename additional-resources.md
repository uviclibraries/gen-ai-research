---
layout: default
title: Additional Resources
nav_order: 10
---
# Additional Resources & Acknowledgements

## Generative AI Prompt Design
<img src="images/ai-usage-label.png" style="float: right;" width = "300px">
The [**AI Usage Label**](https://ailabel.netlify.app/){:target="_blank"} is a free tool was developed & made available by [Dr. Faraz Forghan Parast](https://etcl.uvic.ca/2023/11/16/meet-the-etcl-team-faraz-forghan-parast/){:target="_blank"} who is a Fellow at the University of Victoria, [Electronic Textual Cultures Lab](https://etcl.uvic.ca/2023/11/16/meet-the-etcl-team-faraz-forghan-parast/){:target="_blank"} (ETCL).

## Acknowledgements

- [Generative AI Presentation by Scott Cowan MLIS, Roger Reka MI](https://docs.google.com/presentation/d/1IVFsg0qVdbdc3ESvvihDYQYpCMAxzNiVvIG5LIoOWos/){:target="_blank"} (CC-BY), from the Leddy Library at the University of Windsor
- Christian Schmidt, [Artificial Intelligence library guide](https://libguides.uvic.ca/AI_Tools){:target="_blank"} (CC-BY-SA), from the University of Victoria Libraries
- Rich McCue & Zarah Premji presentation: [Generative AI & Academic Assignments: Exclude or Embrace?](https://docs.google.com/presentation/d/1Z7ulU4r8YO4AfHlRwaXLkTzM0V3rxN2bAo7aAD9S_jg/){:target="_blank"} (CC-BY)
- [UBC Library Research Commons](https://github.com/ubc-library-rc/){:target="_blank"}, for their assistance with the Jekyll template for GitHub Pages.

# Additional Resources

## Debugging playbook (why outputs suck, and the exact fix)
Use this when the model gives you nonsense.

### Problem: Too vague / generic
**Fix prompt:**  `Ask me 3 clarification questions first. Then produce the output using my answers.`

### Problem: Hallucinated facts / made-up citations
**Fix prompt:**  `List each factual claim as a bullet. For each claim: give a source URL + date. If you can’t, write “UNVERIFIED.” Then rewrite using only VERIFIED claims.`

### Problem: Too long / rambling
**Fix prompt:**  `Rewrite to <=90 words. Keep only the top 3 points. Remove examples and filler.`

### Problem: Wrong level for audience
**Fix prompt:**  `Rewrite for <audience>. Add 1 simple example. Remove technical jargon.`

### Problem: Scope creep (“everything about X”)
**Fix prompt:**  `Limit to: <3–5 specific subtopics>. One sentence each. No extras.`

## Privacy & safety
- UVic guidance on GenAI in research
- Redaction/metadata tools (exhilaration tool, Office “Inspect Document”)

## Research workflows
- Zotero, ResearchRabbit/Connected Papers (always verify)
- Query syntax cheat sheets (Boolean, truncation, phrase search)
- Disclose use of AI in research: https://ailabel.netlify.app/

> Keep this short and vetted. Remove anything dead or duplicated.


[NEXT STEP: Workshop Evaluation Survey](workshop-survey.html){: .btn .btn-blue }
