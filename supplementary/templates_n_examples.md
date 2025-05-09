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
