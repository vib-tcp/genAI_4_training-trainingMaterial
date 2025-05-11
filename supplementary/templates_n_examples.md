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

# Create narratives to slides

Giving the PDF of the slides AI should suggest the narrative to be explained in each slide. Supporting trainers with slide nnotation and increasinf FAIRness.

### PROMPT:

Read the PDF document. For each slide give a header and a clear, concise and explanatory narrative. The narrative should be writen in the 1st person, like if I was teaching. Include the explanation of illustrations when there are in the slide.

### RESULTS:

Here’s a slide-by-slide breakdown of the PDF **"0_introduction 1.pdf"**, written in the **first person** as if you were teaching the material. Each slide includes a **header**, a **clear narrative**, and **explanations of illustrations** where applicable.

---

### **Slide 1: Introduction to Cancer Classification**
**Narrative:**  
Let me start by introducing the problem we're tackling: classifying lesions as either **malignant** or **benign** using image data. On this slide, you can see two rows of images—**the top row shows malignant lesions**, and **the bottom row shows benign ones**.  
To make this classification, we extract **features** from the images—these are measurable properties like shape or texture. Each image becomes a **sample** in our dataset, and each sample has a **label** indicating whether it's malignant or benign. This is the foundation of our machine learning pipeline.

---

### **Slide 2: Understanding Key Terms**
**Narrative:**  
Before we dive deeper, let’s clarify some terminology. A **feature** is a measurable attribute—like the roundness of a lesion. A **sample** (also called an instance or data point) is one example in our dataset. And the **label** is the known outcome we’re trying to predict—malignant or benign. These terms are essential for understanding how supervised learning works.

---

### **Slide 3: Using Eccentricity as a Feature**
**Narrative:**  
Now, let’s look at a specific feature: **eccentricity**, which measures how circular a lesion is. A perfect circle has an eccentricity of 0, and more elongated shapes have values closer to 1.

We have two histograms here:
- The **left histogram** shows the distribution of eccentricity values for **malignant lesions**. Notice how the values are generally higher—these lesions tend to be more elongated.
- The **right histogram** shows the distribution for **benign lesions**, which are more circular and thus have lower eccentricity values.

This visual difference suggests that eccentricity could be a useful feature for distinguishing between the two classes.

---

### **Slide 4: Threshold-Based Classification**
**Narrative:**  
Let’s see how we can use eccentricity to classify lesions. We set a **threshold value (t)**—if a lesion’s eccentricity is greater than **t**, we classify it as malignant; otherwise, it’s benign.

The **histogram** here shows how lesions are distributed around the threshold. By adjusting **t**, we can control how many lesions fall into each category.

The **table** is a **confusion matrix**, which summarizes the outcomes:
- **True Positives (TP):** Malignant lesions correctly classified.
- **False Negatives (FN):** Malignant lesions incorrectly classified as benign.
- **False Positives (FP):** Benign lesions incorrectly classified as malignant.
- **True Negatives (TN):** Benign lesions correctly classified.

This helps us evaluate how well our classifier is performing.

---

### **Slide 5: Evaluating Classifier Performance**
**Narrative:**  
To assess our classifier, we use metrics derived from the confusion matrix:
- **Accuracy** measures overall correctness.
- **True Positive Rate (TPR)** tells us how many actual malignant cases we correctly identified.
- **False Positive Rate (FPR)** tells us how many benign cases we incorrectly labeled as malignant.

These metrics help us understand the trade-offs involved in choosing a threshold.

---

### **Slide 6: ROC Curve and AUC**
**Narrative:**  
Here, I introduce the **ROC curve**—a plot of TPR versus FPR for different threshold values. It shows how the classifier’s performance changes as we vary the threshold.  
The **Area Under the Curve (AUC)** is a single number summarizing performance. A value close to 1 means excellent classification. In our example, the AUC is 0.98, which is very good.

---

### **Slide 7: Adding More Features**
**Narrative:**  
To improve classification, we can add another feature—**solidity**, which measures how compact a lesion is. Now, each sample is represented by a **feature vector** in a 2D space (eccentricity and solidity). This allows us to draw more complex decision boundaries and improve accuracy.

---

### **Slide 8: Linear SVM Classification**
**Narrative:**  
Here, I use a **Linear Support Vector Machine (SVM)** to classify lesions in the 2D feature space. The plot shows a **linear decision boundary**—everything on one side is classified as malignant (blue), and the other side as benign (red). This is a simple yet effective approach when the data is linearly separable.

---

### **Slide 9: Decision Trees for Nonlinear Boundaries**
**Narrative:**  
When the data isn’t linearly separable, we can use a **Decision Tree**. This model creates a nonlinear decision boundary by splitting the feature space into regions. It’s especially useful when we have more features and more complex patterns in the data.

---

### **Slide 10: Generalization and Overfitting**
**Narrative:**  
It’s important that our model performs well not just on training data, but also on **unseen external images**. This is called **generalization**. If the model is too complex, it might memorize the training data and fail on new data—a problem known as **overfitting**.

---

### **Slide 11: Data Normalization**
**Narrative:**  
When we use multiple features, they might be on different scales. For example, eccentricity might range from 0 to 100, while solidity ranges from -5 to 7. To ensure each feature contributes equally, we apply **data normalization**.

We can use:
- **Standardization**: Rescales features to have mean 0 and standard deviation 1.
- **Min-max scaling**: Rescales features to a fixed range, like [0, 1].

This step is crucial for many machine learning algorithms.

---

### **Slide 12: Visualizing Eccentricity Distributions in Python**
**Narrative:**  
Here, I use Python to load the eccentricity dataset and plot the distributions for malignant and benign lesions using **Seaborn**. The blue curve represents malignant cases, and the green curve represents benign ones. This visualization confirms what we saw earlier—malignant lesions tend to have higher eccentricity.

---

### **Slide 13: Confusion Matrix in Python**
**Narrative:**  
Using **Scikit-learn**, I compute the confusion matrix for a threshold of 0.7. The matrix shows:
- 40 true positives
- 10 false negatives
- 0 false positives
- 50 true negatives

This gives us a clear picture of how well our classifier is performing.

---

### **Slide 14: ROC Curve in Python**
**Narrative:**  
Next, I plot the **ROC curve** using Scikit-learn. The curve rises quickly toward the top-left corner, indicating high sensitivity and specificity. The **AUC is 0.9792**, which confirms excellent performance.

---

### **Slide 15: Feature Space Visualization**
**Narrative:**  
This plot shows the 2D feature space with **eccentricity** on the x-axis and **solidity** on the y-axis. Each point is colored by its label—malignant or benign. This helps us visually assess how well the features separate the two classes.

---

### **Slide 16: Decision Tree Boundary in Python**
**Narrative:**  
I train a **Decision Tree Classifier** and plot its decision boundary. The model achieves **99% accuracy**, and the boundary clearly separates the two classes in the feature space. This shows how powerful decision trees can be for nonlinear classification.

---

### **Slide 17: Boxplot of Unscaled Features**
**Narrative:**  
Finally, I show a **boxplot** of unscaled gene expression features. You can see that the features vary widely in scale. This reinforces the need for normalization before feeding the data into a machine learning model.

---

Would you like me to turn this into a presentation or teaching script?



Here’s a bullet point list of the EU Research Competences (ResearchComp):

# Evaluate courses in relation to European Competence Framework for Researchers (ResearchComp) 

In this case best result arised from a combined and ste-by-step procedure.

### STEP 1:

REading the files and preventing AI to print all the files in the screen.

** PROMTP 1:**

Add summary.pdf and syllabus.pdf.
Read both files and give me a 3 lines summary of each 

** RESULT 1:**

Here are the 3-line summaries for each document:

### **ML_Copilot_summary 1.pdf**
- The document introduces a binary classification task in medical imaging, distinguishing between malignant and benign lesions using feature vectors.
- It explains feature extraction, model thresholding, and the impact of decision boundaries on model complexity and overfitting.
- Emphasis is placed on generalization, normalization, and scaling to ensure robust and fair model performance.

### **description 1.pdf**
- This is a 2-day Machine Learning & Deep Learning workshop organized in Ghent for VIB researchers and staff.
- It requires basic Python knowledge, with an optional crash course available for beginners.
- No prior experience in machine learning is needed—just a strong interest in the topic.

Would you like a visual summary or a comparison between the two?

### STEP 2

**PROMPT 2:**
list the high level topics for research comp of the european competency

**RESULT 2:**
The **European Competence Framework for Researchers (ResearchComp)** outlines seven high-level research competency areas:

1. **Cognitive Abilities** – Includes abstract, critical, analytical, strategic, and systemic thinking, as well as creativity and problem-solving.
2. **Doing Research** – Covers disciplinary expertise, conducting scientific and interdisciplinary research, writing research documents, and applying ethics and integrity.
3. **Managing Research** – Involves project management, resource mobilization, evaluation, negotiation, and promoting open access.
4. **Managing Research Tools** – Focuses on data management, intellectual property, citizen science, and use of open-source tools.
5. **Making an Impact** – Encompasses dissemination, teaching, public communication, policy influence, and innovation.
6. **Working with Others** – Includes teamwork, networking, mentoring, inclusion, and professional interaction.
7. **Self-Management** – Covers personal development, entrepreneurship, stress management, and self-organization [1](https://research-and-innovation.ec.europa.eu/jobs-research/researchcomp-european-competence-framework-researchers_en).

Would you like a visual map or a breakdown of each area with examples?

### STEP 3

**PROMPT 3:**

taking in consideration only the content in the files. Evaluate if the course can fit any of the RsearchComp. If so, name the topic and add an explanation to justify the suggestion. List only the ones which fit clearly within this course.

**RESULT 3:**
Based on the content of the two documents, the course clearly aligns with the following **ResearchComp** competency areas:

---

### **1. Doing Research**
**Topic:** *Conducting scientific research and applying disciplinary knowledge*

**Justification:**  
The course introduces participants to medical image classification using machine learning, including feature extraction, model evaluation, and generalization. These are core components of conducting scientific research in data-driven disciplines.

---

### **2. Managing Research Tools**
**Topic:** *Using digital tools and data management techniques*

**Justification:**  
The course involves Python programming, data normalization, and model evaluation techniques—skills essential for managing research data and using computational tools effectively in modern research environments.

---

Would you like me to map these to specific learning outcomes or suggest how to present this alignment in a report or presentation?

## Draft some nalogies for a topic

Using the summary or not you can ask AI to support you with some creative hints to connect with the students.

### PROMPT:

You are an expert tutor in post-grad level, helping me explain an exercise in machine learning.
Come up with 3 creative analogies to explain data normalization, using analogies drawn from a contemporary popular culture. Make these analogies meaningful for a diverse nationality post-grad students community living in europe.

### Observations

Possible iterations that can improve results.

a.) Suggest some counterexamples that work against the analogy.

b.) What are some ways these analogies work? Provide concrete example.


### RESULT

Absolutely! Here are **three creative analogies** for explaining **data normalization** using references from **contemporary popular culture**, tailored for a **diverse, international post-grad community in Europe**:

---

### **1. Netflix Subtitles: Making Dialogue Universally Understandable**

**Analogy:**  
Imagine watching *Stranger Things* on Netflix with friends from different countries. The characters speak fast, use slang, and have strong American accents. Without subtitles, it’s hard for everyone to follow. Subtitles **normalize** the dialogue — they bring it to a common, understandable format for all viewers, regardless of language or hearing ability.

**How it relates to data normalization:**  
Just like subtitles make diverse speech patterns understandable to a global audience, **normalization transforms data from different scales into a common scale**, so machine learning models can "understand" and compare them fairly.

---

### **2. FIFA Video Game Player Stats: Leveling the Playing Field**

**Analogy:**  
In *FIFA 24*, players from different leagues and countries have stats like speed, stamina, and shooting rated on different scales. To create a balanced "Ultimate Team," the game **normalizes** these stats so that a 90 in speed for Mbappé means the same as a 90 in speed for Haaland.

**How it relates to data normalization:**  
Just like FIFA ensures that stats are comparable across players, **data normalization ensures that features like income, age, or height don’t unfairly dominate** just because they’re measured in different units or scales.

---

### **3. Eurovision Song Contest Voting: Fair Scoring Across Countries**

**Analogy:**  
In Eurovision, each country gives points to their favorite songs. But countries have different populations, cultures, and biases. To make the scoring fair, the system **normalizes** votes — each country gives the same number of points, regardless of size or preference intensity.

**How it relates to data normalization:**  
Just like Eurovision ensures that no country’s vote outweighs another’s, **normalization ensures that no single feature dominates a machine learning model** just because it has a larger numeric range.

---

Would you like a visual infographic or slide version of these analogies for a presentation or class discussion?
