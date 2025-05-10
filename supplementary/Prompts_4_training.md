# Prompt Library to increase FAIRness in training material with support of AI

Provide filet to AI. For this example the sample used was from ["Machine Learning Course 2day"](https://github.com/sdgroeve/Machine-Learning-Course-2days) from Sven Degroeve. Slide [_0_introduction.pdf_](https://github.com/sdgroeve/Machine-Learning-Course-2days/blob/main/slides/0_introduction.pdf).
For this example was used Copilot. This test was run in May 2025.

**This prompts were inspired by:**

[AI 4 Education prompt library](https://www.aiforeducation.io/prompts)

[Summary with AI, Maastricht University](https://library.maastrichtuniversity.nl/apps-tools/ai-prompt-library/summarise-with-ai-prompts/)

[Strategic use of generative AI course from VIB](https://github.com/vibbits/introduction-to-generative-ai/blob/main/supplementary/prompting-templates-Morningactivity.md)



## 1. Get a summary of the course

This procedure will define the context of the AI session.

### PROMPT:

Act as a professional summarizer. Create a concise and comprehensive summary of the pdf, while adhering to the guidelines below.

Guidelines:  

1- Create a summary that is detailed, thorough, in-depth, and complex, while maintaining clarity and conciseness

2- The summary must cover all the key points and main ideas presented in the original text, while also condensing the information into a concise and easy-to-understand format

3- Ensure that the summary includes relevant details and examples that support the main ideas, while avoiding any unnecessary information or repetition

4- Rely strictly on the provided text, without including external information

5-The length of the summary must be appropriate for the length and complexity of the original text. The length must allow to capture the main points and key details,

6-Ensure that the summary is well-organized and easy to read, with clear headings and subheadings to guide the reader through each section. Format each section in paragraph form


## 2. Draft the Learning Outcomes using Blooms Taxonomy

You can use a new prompt to copy the summary done in the session before or after saving into a file you can provide the PDF file again to AI. It is possible to do in the same prompt, but if the AI has started creating in the syllabus it can influence the result. A clean start could guide to cleaner results.

### PROMPT:

You are now an expert teacher in Machine Learning, experienced in developing lesson plans, and educational frameworks for effective and meaningful learning. 

Your task is, based on the PDF summary and Syllabus to suggest 3 learning outcomes for each of the Bloom’s Taxonomy levels. Take into account the definition of the adiance to create appropriate outcomes. Format as bulleted list and includ in bold and in parenthesis by the end of the learning outcome to which level of the Blooms taxonomy its relates. 

Consider the revised Blooms taxonomy from 2021. For each topic include one example of activity that the trainer could use to assess if the learning outcome was achieved by the student.

## 3. Draft a lesson syllabus

To draft a syllabus taking in account the VIB template and minimum requirements. 

### PROMPT 1

I want you to support me in writting the syllabus of my lesson.
Based on the item I'm listing in the guidelines, I want you to read the pdf and fill up the field.
If the information cannot be found in the file refrain of assuming or creating answers. Describe it as missin information. After you do the first taks, ask one question at the time, to fill up the missing fields based on my answer.

Before we start greet me and ask me for the pdf file.

Guidelines:

1. Title
2. Description. One concize paragraph to desribe the general context of the lesson. It should be engaging and atractive. But casual.
3. Include the learning outcomes (Blooms taxonomy) in a topic format and with the blooms level in parenthesis and bold at the end of each topic.
4. Target audiance
5. Prerequisites in a list. Classify them as Technical or Knowledge.
6. Trainers list
7. Course level (Begginer; Intermediate; Advanced)
8. License (Creative commons)
9. Funding
10. Authors list

### PROMPT 2

You are an expert teacher in Machine Learning, proficient in creating engaging, well-developed and effective lesson syllabus for your students. Your task is to come up with the course syllabus based on the summary and description. Use only the information in the files, refrain of usgin any other information or assuming anythin. The syllabus of this lesson should be engaging and appropriate for PhD and Post-docs students. The syllabus should be written containing all the item in the guidelines and in this order. If an information is missing write "missing info".

Guidelines:

1. Title
2. Description. One concize paragraph to desribe the general context of the lesson. It should be engaging and atractive. But casual.
3. Include the learning outcomes (Blooms taxonomy) in a topic format and with the blooms level in parenthesis and bold at the end of each topic.
4. Target audiance
5. Prerequisites in a list. Classify them as Technical or Knowledge.
6. Trainers list
7. Course level (Begginer; Intermediate; Advanced)
8. License (Creative commons)
9. Funding
10. Authors list


## 4. Create narratives to slides

Giving the PDF of the slides AI should suggest the narrative to be explained in each slide. Supporting trainers with slide nnotation and increasinf FAIRness.

### PROMPT:

Read the PDF document. For each slide give a header and a clear, concise and explanatory narrative. The narrative should be writen in the 1st person, like if I was teaching. Include the explanation of illustrations when there are in the slide.

## 5. Evaluate courses in relation to European Competence Framework for Researchers (ResearchComp) 

In this case best result arised from a combined and ste-by-step procedure.

Reading the files and preventing AI to print all the files in the screen. Use Syllabus, and summary files for this.

### PROMPT 1:

Add summary.pdf and syllabus.pdf.
Read both files and give me a 3 lines summary of each 

### PROMPT 2:

List the high level topics for research comp of the european competency

### PROMPT 3

taking in consideration only the content in the files. Evaluate if the course can fit any of the RsearchComp. If so, name the topic and add an explanation to justify the suggestion. List only the ones which fit clearly within this course.
