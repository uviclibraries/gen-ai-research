---
layout: default
title: 3 - Critically Review
nav_order: 5
parent: Workshop Activities - Introduction
customjs: http://code.jquery.com/jquery-1.4.2.min.js
---
<img src="images/3-critical-review-student.png" style="float:right;width:320px;height:320px;" alt="A student critically reviewing output from a GenAI tool on their laptop."> 

# Critically Review All GenAI Output for Errors
We know that GenAI tools will confidently make factual errors in their statements (or hallucinate). In this section, we will look at some tips so how do we can find those errors, and how we can craft our prompts to help GenAI tools make fewer errors. 

## Be Aware of Traning Data Bias
Generative AI training data bias occurs when the data used to train the AI model reflects societal biases or lacks diversity, sometimes leading to skewed or unfair outputs (ChaGPT 4.0, 2024). Some of the root causes include: 

  - **Culture of the source of training data**, which is largely US-centric at the moment
  - **Underrepresentation of certain groups** like visible minorities and gender bias
<img src="images/3-white-ceos.jpeg" style="float:right;width:320px;height:320px;" alt="3 white male ceo's"> 
  - **Racial & gender bias** in images: Ask Copilot for an image of 3 CEO's and it will probably create a picture of 3 male presenting, white people in suits, which is not representative
  - **Lack of complete data** because not all information is freely accessible on the internet to general-purpose GenAI tools like Copilot, Gemini, and ChatGPT
  - **Historical biases** embedded in the data sources.

We can try to counteract some of these biases by modifying our prompts. Here are some examples you can try in Copilot:
  - **Gender and racial bias**: ```Create an image of 3 CEO's and make them gender and ethnically diverse```
  - **Cultural bias**: ```From a Canadian perspective what key events happened when Great Britain invaded Washington DC in the war of 1812? Privide citations.```

## Prompt Design Tips
Let's look at some ways we can modify our prompts to reduce the number of errors GenAI tools make in response to our prompts ([ChaGPT 4.0, 2024](https://chat.openai.com/share/44bebe63-7c14-49bc-8e2b-e5fac9c6f301){:target="_blank"}):
1. **Ask for Sources**: When possible, ask the model to provide sources or citations for the information it provides. While this is not foolproof, it can help you identify if the information is based on existing knowledge.
  - ```Can you provide a source for your claim that the Great Wall of China is visible from space?```
2. **Consistency Check**: Ask the same question in different ways or at different times to see if the model provides consistent answers. Inconsistent answers may indicate a hallucination.
  - If ChatGPT says that water boils at 100°C at sea level, ask the same question at a later time or in a different way to see if the answer remains consistent.
3. **Use Specific Prompts**: When querying the model, use specific and detailed prompts to reduce the likelihood of the model generating irrelevant or fabricated information. Try these:
  - Instead of asking, ```Tell me about World War II```, ask, ```What were the causes of World War II, and can you list the main countries involved?```

## Critical Review Tips

Critically reviewing the outputs of language models like ChatGPT and Gemini can be challenging, but here are some strategies you can use ([ChaGPT 4.0, 2024](https://chat.openai.com/share/44bebe63-7c14-49bc-8e2b-e5fac9c6f301){:target="_blank"}):

1. **Cross-Verify Facts**: Cross-check the information provided by the model with reliable sources. If the information is inconsistent or cannot be found in reputable sources, it might be a hallucination.
  - For instance, if ChatGPT claims that Toronto is the capital of Canada, cross-check with a reputable source like a government website or a geography textbook to verify that Ottawa is actually the capital.
3. **Cross-Verify Citations**: Check to make sure that for each citation (and don't forget to ask for sources):
  - The source exists whether it be a web page, book, or journal article.
  - The quotation or summary exists and is fairly represented by the GenAI tool.
3. **Expert Review**: If you have access to subject matter experts, have them review the model's output for accuracy and reliability. Even easier if you are a subject matter expert.
4. **Model Limitations Awareness**: Be aware of the limitations of the model you are using. Understanding the types of errors or hallucinations a model is prone to can help you identify them more easily.
  - Be aware that ChatGPT may struggle with very recent events or highly specialized knowledge, so take its answers in these areas with caution. In academic research specifically, please be aware that General GenAI tools do not have access to research papers behind paywalls, so in disciplines like Law where almost all peer review information (like legal commentaries) are behind paywalls, general GenAI tools perform very poorly.
8. **Critical Thinking**: Apply critical thinking skills to evaluate the plausibility and coherence of the model's responses.
  - For example, if a GenAI tool claims that humans can live without water for a month, apply critical thinking to question the plausibility of this statement based on known human biology.

Remember, while these strategies can help reduce the likelihood of encountering hallucinations, no method is foolproof. Always use multiple sources and verification methods when relying on information provided by language models.

## Let's Practice!
1. Choose a topic that you know a lot about. For example: I know a lot about the manager of the DSC, Rich McCue.
2. Ask your GenAI tool a few questions about a topic that you know the answers to. For Example: ```What is Rich McCue from the University of Victoria known for?```
  - Copilot's response: "Rich McCue is known for managing the University of Victoria Libraries Digital Scholarship Commons, where he helps students, faculty, and staff learn to create accessible scholarly communications. He provides digital tools like 3D printers, electronics kits, Virtual Reality equipment, and data visualization software, and teaches people how to use them. Rich is also a sessional instructor in the Faculty of Education at the University of Victoria, where he teaches educational technology-related classes to undergraduate students. His research interests include informal credentialing, active learning pedagogies, flipped learning, makerspaces, and open learning​​​​. Additionally, Rich is pursuing a Masters of Arts in Education with Dr. Valerie Irvine, focusing on exploring the relative effectiveness of blended classroom / project-based pedagogy compared to a lecture-based pedagogy for information literacy instruction​​."
4. How did your GenAI tool do for this question? Not bad, in that it is almost completely correct, except that it says that Rich McCue is "pursuing a Master of Arts in Education." In reality, Rich earned that degree 8 years ago. So close, but not 100% accurate.
> Note: If you use information from a GenAI tool for an assignment with mistakes that you repeat, it will lower your grade.

## Reflection time:
> - **How did your GenAI tool do when it answered your questions? Any inaccuracies?**
> - **How will you try to craft your prompts to make the response less biased and more inclusive?**
> - **What are the key things you can do to critically review GenAI generated responses?**

[NEXT STEP: Cite GenAI Output](4-cite.html){: .btn .btn-blue }
