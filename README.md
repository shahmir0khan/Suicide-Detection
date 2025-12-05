#Suicide Risk Detection Model (Final-Year Project Component)

This project is a key module of my **Multimodal AI Psychologist System**, designed to identify suicidal intent in user-generated text.  
Using **200k+ Reddit posts**, a custom NLP pipeline, and a fine-tuned **ELECTRA transformer**, the model achieves **97% accuracy** in detecting crisis language.

---

##  Project Overview

The goal of this project is to convert real, messy social media data into **clean, reliable predictive insights**.  
This mirrors real-world analytics challenges where unstructured user data must be transformed into actionable information.

---

##  Dataset

- **Source:** Reddit suicide-watch and mental-health communities  
- **Size:** 200,000+ posts  
- **Cleaning:**  
  - Removed duplicates and irrelevant text  
  - Handled missing values  
  - Controlled extreme post-length outliers using the **75th percentile (155 words)**  
  - Ensured balanced training data

---

##  Preprocessing Pipeline

A customized NLP cleaning pipeline designed specifically for social media text:

- Preserved negations (*no, not, never*)
- Lemmatized text while keeping semantic meaning
- Removed URLs, emails, special characters, and emojis
- Tokenized and encoded text for model consumption
- Exploratory analysis via:
  - Word clouds
  - Bigrams
  - Sentiment distribution

These steps confirmed that suicidal posts exhibited distinct linguistic patterns.

---

##  Model Architecture

**Model Used:** ELECTRA (transfer learning)

### Why ELECTRA?
- Efficient transformer architecture  
- Strong performance on downstream NLP tasks  
- Faster training compared to BERT/RoBERTa  

### Training Highlights:
- Fine-tuned on preprocessed Reddit text  
- Binary classification: *Suicidal vs. Non-suicidal*  
- Evaluated using accuracy, precision, recall, F1-score

**Final Accuracy:** **97%**

---

##  Results

| Metric      | Score |
|-------------|--------|
| Accuracy    | 98%    |
| Precision   | 98%    |
| Recall      | 98%    |
| F1-Score    | 98%    |

The model successfully identifies crisis-related language with high reliability.

---

##  Tech Stack

- **Python**
- **Transformers (HuggingFace)**
- **PyTorch / TensorFlow**
- **Scikit-learn**
- **Pandas**
- **Matplotlib / Seaborn**
- **NLTK / spaCy**


