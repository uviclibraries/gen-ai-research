---
layout: default
title: 3 - Critically Review
nav_order: 5
parent: Workshop Activities - Introduction
customjs: http://code.jquery.com/jquery-1.4.2.min.js
---
<img src="images/CHANGE_ME.png" style="float:right;width:320px;height:320px;" alt="????"> 

# Critically Review All GenAI Output for Errors
We know that GenAI tools will confidently make factual errors in their statements (or hallucinate). In this section we will look at some tips so how do we can find those errors, and what we can craft our prompts to help GenAI tools make fewer errors. 

If you have any questions or get stuck as you work through this in-class GenAI exercise, please ask the instructor for assistance.  Have fun!

## Prompt Design Tips
Let's look at some ways we can modify our prompts to reduce the number of errors GenAI tools make in response to our prompts ([ChaGPT 4.0, 2024](https://chat.openai.com/share/44bebe63-7c14-49bc-8e2b-e5fac9c6f301){:target="_blank"}):
1. Ask for Sources: When possible, ask the model to provide sources or citations for the information it provides. While this is not foolproof, it can help you identify if the information is based on existing knowledge.
  - <br>```Can you provide a source for your claim that the Great Wall of China is visible from space?```<br>
2. Consistency Check: Ask the same question in different ways or at different times to see if the model provides consistent answers. Inconsistent answers may indicate a hallucination.
  - <br>```sample prompt here```<br>
3. Use Specific Prompts: When querying the model, use specific and detailed prompts to reduce the likelihood of the model generating irrelevant or fabricated information.
  - <br>```sample prompt here```<br>
  - Instead of asking, ```Tell me about World War II```, ask, ```What were the causes of World War II, and can you list the main countries involved?```

## Critical Review Tips

Critically reviewing the outputs of language models like ChatGPT and Gemini can be challenging, but here are some strategies you can use ([ChaGPT 4.0, 2024](https://chat.openai.com/share/44bebe63-7c14-49bc-8e2b-e5fac9c6f301){:target="_blank"}):

1. **Cross-Verify Facts**: Cross-check the information provided by the model with reliable sources. If the information is inconsistent or cannot be found in reputable sources, it might be a hallucination.
  - For instance, if ChatGPT claims that Toronto is the capital of Canada, cross-check with a reputable source like a government website or a geography textbook to verify that Ottawa is actually the capital.
3. **Cross-Verify Citations**: Check to make sure that for each citation:
  - The source exists whether it be a web page, book, or journal article.
  - The quotation or summary exists and is fairly represented by the GenAI tool.
3. **Expert Review**: If you have access to subject matter experts, have them review the model's output for accuracy and reliability. Even easier if you are a subject matter expert.
4. **Model Limitations Awareness**: Be aware of the limitations of the model you are using. Understanding the types of errors or hallucinations a model is prone to can help you identify them more easily.
8. **Critical Thinking**: Apply critical thinking skills to evaluate the plausibility and coherence of the model's responses.

Remember, while these strategies can help reduce the likelihood of encountering hallucinations, no method is foolproof. Always use multiple sources and verification methods when relying on information provided by language models.
