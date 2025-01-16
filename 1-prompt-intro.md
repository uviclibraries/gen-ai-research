---
layout: default
title: 1 - Prompt Design Intro
nav_order: 3
parent: Workshop Activities
customjs: http://code.jquery.com/jquery-1.4.2.min.js
--- 

# Prompt Design Introduction
<img src="images/prompt-design-image.png" style="float:right;width:320px;" alt="A student at a computer learning effective GenAI prompt design">
If you have any questions or get stuck as you work through this in-class GenAI exercise, please ask the instructor for assistance.  Have fun!

## Prompt Design Basics: The CRAFT Framework
While it is easy to get started using Generative AI tools, it takes time and practice to get the best results out of Generative AI tools. 
Each element of the CRAFT framework below contributes to the overall effectiveness of your prompt, making sure that the outputs are clear, relevant, and well-structured:
- **Context**: Set the stage by providing background information. Include key details like the purpose of the task, audience, or tone. Example: ```Write a formal email to a professor about missing class due to illness.```
- **Role**: Specify the perspective or role the AI should take on. Example: ```Act as a historian explaining the causes of the French Revolution.```
- **Action**: Clearly describe the specific action or outcome you want. Example: ```Summarize the main points of this article in two paragraphs.```
- **Format**: State the structure or format of the response (e.g., list, essay, dialogue). Example: ```Provide the answer in bullet points for easy reading.```
- **Targe Audience**: Identify who the output is intended for, which can affect tone and style. Example: ```Write for a high school student unfamiliar with this topic.```

### Let's Practice!
1. If you haven't already, in your favourite web browser please open either [**Perplexity.ai**](https://www.perplexity.ai/){:target="_blank"} (no account required) -OR- [**Microsoft Copilot**](https://copilot.microsoft.com/){:target="_blank"}. If you are a UVic student you can use a version of Copilot licensed for you by UVic by logging on with your UVic email address (e.g. _noahsmith@uvic.ca_). The UVic version of Copilot runs on servers located in Canada and does not share any of the prompts you create with Microsoft, or resulting data for training data, which is great from a privacy perspective. Perplexity is a great option if you don't want to use a login, but does not allow you to generate images like the UVic version of CoPilot.
> Note: You are free to use other GenAI tools for this workshop but please note that you will either have to create accounts for most of these services if you have not already done so, and will need to take extra steps to preserve your privacy if privacy is important to you:
>  - [ChatGPT](https://chat.openai.com/){:target="_blank"}
>  - [Meta.ai](https://www.meta.ai/){:target="_blank"}
>  - [Claude.ai](https://claude.ai/){:target="_blank"}
>  - [Google Gemini](https://gemini.google.com/){:target="_blank"} 
2. Test a poor prompt to start with. Copy and paste the following text into your GenAI tool and note the results:<br>
```Tell me about the weather.```<br>
<br><img src="images/prompt-lesson-poor.png"  alt="An image of Copilot with a weather poor weather prompt example"><br>
  - What are the results from this prompt telling you?
3. Now let's try a prompt that includes more details relevant to the hypothetical help we need to create a lesson plan and activity for a grade 2 class by copying and pasting the following text into your GenAI tool:
<br>```I am a teacher teaching grade 2 students about the weather. Please assume the role of a teacher and generate a lesson plan in bullet point form for a one-hour lesson about weather including a 30-minute activity to help students remember what they learned in the instruction portion of the lesson. The activity instruction should be at a grade 2 level. Please provide sources.```<br>
<br><img src="images/1-prompt-weather-lesson.png"  alt="An image of Copilot with a weather lesson prompt example"><br>
>  - **How does the response to this prompt differ from the "_poor_" prompt above?**
>  - **Do you have the weather-related expertise to determine if the weather-related facts are accurate?**
>  - **Do you have the teaching expertise to know if the weather lesson plan is reasonable and will work well with grade 2 students?**
> <br>_Note: every time we use GenAI tools we should ask ourselves whether or not we have the expertise to evaluate the accuracy of GenAI-generated text, because as we know they are not always accurate or factual._
4. Pick one or two topics that you know a lot about (e.g. ```What are the origins of skateboarding?```). 
>  - **Ask Perplexity.ai -or- Microsoft Copilot a question about one of the topics.**
>  - **Is the answer accurate?**
>  - **Can you make it more accurate with follow-up prompts?**
>  - **Ask Copilot a question about your second topic.**
>  - **How did it do for each topic?**
>     - **Was it completely accurate?**
>     - **Did you have to research to verify any of the claims Copilot made?**
<br>
> **NOTE: If you'd like to earn a workshop badge, please take a picture or screenshot of the prompt and output of one of the tropics you know a lot about as this is one of the criteria to earn a workshop badge.**


## Let's Practice Idea Generation!
> Please remember that **you must have permission from your instructor to use GenAI to assist you in any class assignment**. Your instructor may forbid the use of GenAI, allow limited use of GenAI, or all full use of GenAI for specific assignments. Please follow your instructors' guidelines for how to cite and document your use of GenAI in assignments. If you have any questions about using GenAI in your class, please look at your course outline, and if you don't find guidance there, ask your instructor directly, as using GenAI without permission from your instructor is a form of plagiarism and is a violation of UVic's [Academic Integrity Policy](https://www.uvic.ca/students/academics/academic-integrity/index.php). 

Now let's look at how we can use GenAI tools for creativity and innovation, including how to generate new ideas and overcome creative blocks ([ChatGPT 4.0, 2024](https://chat.openai.com/share/ec126ed8-937c-4f48-a322-cebde4bddd55){:target="_blank"}). Type or copy and paste the prompts below into Copilot and then let's look at the results.
1. First let's look at a technique to help us generate possible ideas for undergraduate honours research projects. Note that you probably won't get any truly unique topics suggested by GenAI tools, however, they can be useful for brainstorming and may prompt you to think of other related ideas as you look at what the GenAI tool has suggested.
  - Topic exploration: ```I am an undergraduate student getting ready to start an honours research project. I am interested in university-level academic makerspaces. What are some topics of inquiry that might be interesting for me to research or explore on this topic?```
  - Now try exploring a topic that you are interested in!
2. Research Question Formulation: ChatGPT can assist in refining research questions by providing feedback on clarity, focus, and feasibility.
  - Next, we'll take one of the bullet points from the Topic Exploration output, and add to the beginning of it: "Suggest 5 research questions with measurable outcomes for the following topic:"  This should provide us with ideas for research questions based on the topic. Note that even if you love one of the suggested research questions, you'll almost certainly modify it to suit your specific situation and possibly location. Here is an example:
<br>```Suggest 5 research questions for the following topic: Evaluate the effectiveness of makerspace programs. What assessment methods can be used to measure learning outcomes? How can we assess the impact of makerspaces on students’ employability?```
  - Now try using one of your own generated topics and request it to suggest research questions.
3. Summarize a document, but be very careful as currently (March 2024) **free GenAI tools have limits on the size of documents that they can summarize**. You can ask the GenAI tool to let you know if it can't "read" the whole article to summarize it.
  - Request a summary of an article titled, [LEGO helps Langford man recapture life after induced coma in 2018](https://www.saanichnews.com/local-news/lego-helps-langford-man-recapture-life-after-induced-coma-in-2018-7333837){:target="_blank"}, by opening the article, and copying the text of the article to use in the next step.
<br>```Please summarize the main points in this article. If you cannot summarize the whole article please tell me that you couldn't: https://www.saanichnews.com/local-news/lego-helps-langford-man-recapture-life-after-induced-coma-in-2018-7333837```<br>
  - Follup with the following prompt requesting a more detailed summary:
<br>```Please expand the summary to 5 or more bullet points.```<br>
  - Are the two summaries significantly different? If so in what ways?
  - Now try summarizing one of your own documents, or a web page!
> NOTE: The standard version of Copilot (which UVic has licenced for us) is not able to summarize large bodies of text, including documents over approximately 3,100 characters (as of March 2024). 
4. Reflection Time:
>  - **How useful were the research topic ideas that your GenAI tool created?**
>  - **Do you have enough background knowledge to critically evaluate the quality of Copilot's suggested research topics?**
>  - **How useful were the research questions that GenAI tool created?**
>  - **Did you GenAI tool do a good job in summarizing the document?**
  
## Go further
There are many excellent resources on the internet with tips and tricks for prompt design, to please feel free to go deeper with [articles like this](https://www.geeky-gadgets.com/prompt-engineering-techniques/){:target="_blank"} if you'd like to improve your prompt design skill set.

[NEXT STEP: Intermediate Prompt Design](2-prompt-design-inter.html){: .btn .btn-blue }
