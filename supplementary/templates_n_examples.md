# Prompt Library to increase FAIRness in training material with support of AI

Provide filet to AI. For this example the sample used was from ["Machine Learning Course 2day"](https://github.com/sdgroeve/Machine-Learning-Course-2days) from Sven Degroeve. Slide [_0_introduction.pdf_](https://github.com/sdgroeve/Machine-Learning-Course-2days/blob/main/slides/0_introduction.pdf).
For this example was used Copilot. This test was run in May 2025.


## Get a summary of the course

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
![image](https://github.com/user-attachments/assets/82c14259-2b73-4fee-a99a-56d6f096d726)

### RESULT:

Here's a detailed and well-structured summary of the document **"0_introduction.pdf"**, following your guidelines:

---

## **Introduction to Medical Image Classification and Feature-Based Modeling**

### **1. Medical Image Classification Context**
The document introduces a classification task involving medical images, specifically distinguishing between **malignant** (cancerous) and **benign** (non-cancerous) lesions. The classification is binary:
- **Malignant** is treated as the **positive class**
- **Benign** is the **negative class**

Each image is associated with a **label** (target) and a **feature vector** (a set of measurable properties or attributes extracted from the image).

---

### **2. Feature Extraction and Representation**
Key concepts in feature-based modeling are introduced:
- **Feature extraction** involves identifying measurable characteristics (e.g., **eccentricity**—how circular a lesion is).
- Each image is represented as a **feature vector** in a **Euclidean vector space**, enabling mathematical operations and comparisons.
- The **feature vector X** encapsulates all extracted features for a given image.

---

### **3. Classification Models and Thresholding**
The document discusses how classification models operate:
- A **threshold (t)** is used to decide class membership based on feature values.
- Adjusting the threshold affects the **True Positive Rate (TPR)** and **False Positive Rate (FPR)**:
  - A model classifying all images as malignant yields **TPR = 1, FPR = 1**
  - A model classifying all as benign yields **TPR = 0, FPR = 0**
- The **Area Under the Curve (AUC)** is implied as a performance metric for evaluating model effectiveness across thresholds.

---

### **4. Decision Boundaries and Model Complexity**
- With few features, a **linear decision boundary** can separate classes (e.g., blue region = malignant, red = benign).
- As more features are added, the decision boundary becomes **non-linear and complex**, making it harder to visualize.
- This complexity can lead to **overfitting**, where the model performs well on training data but poorly on **unseen external images**.

---

### **5. Generalization and Overfitting**
- A key goal is **generalization**: the model should perform well on new, unseen data.
- Overfitting occurs when the model captures noise or irrelevant patterns in the training data, reducing its predictive power on new data.

---

### **6. Data Normalization and Scaling**
To ensure fair treatment of features during modeling:
- **Normalization** adjusts feature scales to prevent dominance by features with larger numeric ranges.
- Example: **Eccentricity** might range from [0, 100], while **Solidity** ranges from [-5, 7].
- Techniques include:
  - **Standardization**: transforms features to have zero mean and unit variance.
  - **Min-max scaling**: rescales features to a fixed range (e.g., [0, 1]).

Normalization ensures that all features contribute equally to the model’s decisions.

---

If you'd like, I can also visualize the concepts like decision boundaries or normalization effects. Would you like to explore that next?

## Draft a lesson syllabus

To draft a syllabus taking in account the VIB template and minimum requirements. 

### PROMPT

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

### OBSERVATION & COMMENT

The prompt worked quit well, except that inveted the learning outcomes. Usually it will be added from a different prompt.
Maybe this prompt needs to come after to take into the write direction.

### RESULT

Here is a complete and structured course syllabus based strictly on the content from the provided files:

---

### **1. Title**
**Introduction to Machine Learning & Deep Learning for Medical Image Classification**

---

### **2. Description**
Dive into the world of machine learning and deep learning with this hands-on, beginner-friendly workshop tailored for VIB researchers. Over two days in Ghent, you'll explore how to classify medical images using feature-based models, understand the importance of data normalization, and learn how to build models that generalize well to unseen data. Whether you're a curious newcomer or a seasoned scientist, this workshop offers a practical and engaging entry point into the field.

---

### **3. Learning Outcomes**
By the end of this workshop, participants will be able to:

- Describe the basic principles of binary classification in medical imaging (**Understand**)
- Identify and extract relevant features from medical images (**Apply**)
- Analyze the impact of feature scaling and normalization on model performance (**Analyze**)
- Evaluate classification models using metrics like TPR, FPR, and AUC (**Evaluate**)
- Construct and interpret decision boundaries in low- and high-dimensional feature spaces (**Apply**)
- Recognize and mitigate overfitting in machine learning models (**Understand**)

---

### **4. Target Audience**
- VIB PhD students  
- VIB postdocs  
- VIB staff scientists  
- VIB group leaders or experts  
- VIB technical support staff  

---

### **5. Prerequisites**
**Technical:**
- Basic Python programming (or completion of the crash course in Python)

**Knowledge:**
- No prior knowledge of machine learning required  
- Keen interest in learning ML concepts

---

### **6. Trainers List**
- Robbin  
- Ralf  

---

### **7. Course Level**
**Beginner**

---

### **8. License**
**Creative Commons** (exact type: **missing info**)

---

### **9. Funding**
**missing info**

---

### **10. Authors List**
**missing info**

---

Would you like this syllabus formatted into a downloadable document or presentation?

## Draft the Learning Outcomes using Blooms Taxonomy

You can use a new prompt to copy the summary done in the session before or after saving into a file you can provide the PDF file again to AI. It is possible to do in the same prompt, but if the AI has started creating in the syllabus it can influence the result. A clean start could guide to cleaner results.

### PROMPT:

You are now an expert teacher in Machine Learning, experienced in developing lesson plans, and educational frameworks for effective and meaningful learning. 

Your task is, based on the PDF summary and Syllabus to suggest 3 learning outcomes for each of the Bloom’s Taxonomy levels. Take into account the definition of the adiance to create appropriate outcomes. Format as bulleted list and includ in bold and in parenthesis by the end of the learning outcome to which level of the Blooms taxonomy its relates. 

Consider the revised Blooms taxonomy from 2021. For each topic include one example of activity that the trainer could use to assess if the learning outcome was achieved by the student.

### RESULT:

Based on the summary of the document *"Introduction to Medical Image Classification and Feature-Based Modeling"*, here are **three learning topics for each level of the revised Bloom’s Taxonomy (2021)**, tailored for **PhD students in life sciences**. Each topic includes an example of an assessment activity to evaluate whether the learning outcome (LO) has been achieved.

---

**🔍 Remembering**
- **Topic:** Define key terms in medical image classification (e.g., feature vector, threshold, TPR, FPR).
  - *Assessment:* Multiple-choice quiz on definitions and basic concepts.
- **Topic:** List types of feature scaling techniques (e.g., standardization, min-max scaling).
  - *Assessment:* Flashcard-based recall activity or timed quiz.
- **Topic:** Recall the effects of threshold adjustments on classification outcomes.
  - *Assessment:* Fill-in-the-blank exercise describing TPR and FPR changes with threshold shifts.

---

**🧠 Understanding**
- **Topic:** Explain how feature vectors represent medical images in Euclidean space.
  - *Assessment:* Short written explanation or oral presentation with diagrams.
- **Topic:** Describe the relationship between decision boundary complexity and overfitting.
  - *Assessment:* Concept map creation linking model complexity, visualization, and generalization.
- **Topic:** Interpret the impact of normalization on model fairness.
  - *Assessment:* Annotated example comparing model outputs with and without normalization.

---

**🔧 Applying**
- **Topic:** Apply min-max scaling to a dataset of lesion features.
  - *Assessment:* Hands-on coding task using Python or R to normalize a dataset.
- **Topic:** Use a threshold to classify a small set of medical images based on feature values.
  - *Assessment:* Spreadsheet or script-based classification task with manual threshold tuning.
- **Topic:** Implement a basic linear classifier and visualize the decision boundary.
  - *Assessment:* Jupyter notebook submission with code, plots, and brief interpretation.

---

**🔍 Analyzing**
- **Topic:** Analyze the trade-off between TPR and FPR at different thresholds.
  - *Assessment:* ROC curve plotting and interpretation exercise.
- **Topic:** Compare the effects of different normalization techniques on model performance.
  - *Assessment:* Comparative analysis report using performance metrics (e.g., AUC).
- **Topic:** Deconstruct a model’s decision boundary to identify signs of overfitting.
  - *Assessment:* Case study analysis with visual inspection and justification.

---

**🧠 Evaluating**
- **Topic:** Critique the suitability of linear vs. non-linear models for high-dimensional feature spaces.
  - *Assessment:* Structured debate or peer-reviewed essay.
- **Topic:** Evaluate the generalizability of a model trained on internal vs. external datasets.
  - *Assessment:* Critical review of model performance on cross-validation vs. external test sets.
- **Topic:** Assess the impact of feature selection on classification accuracy.
  - *Assessment:* Experimental design and results interpretation report.

---

**🚀 Creating**
- **Topic:** Design a feature extraction pipeline for a new type of medical image.
  - *Assessment:* Project proposal with rationale, feature list, and expected challenges.
- **Topic:** Develop a visualization tool to demonstrate decision boundaries in 2D feature space.
  - *Assessment:* Interactive tool or dashboard with user guide.
- **Topic:** Construct a research hypothesis on how feature scaling affects model interpretability.
  - *Assessment:* Research abstract and experimental plan submission.

---

Would you like this formatted into a printable lesson plan or teaching guide?
