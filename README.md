# Hw4-tensorflow



**Student:Yeshwanth narige  
id 700764035
  

---

## 📖 Overview  
This repository contains solutions for **Home Assignment 4**  
1. **Q1: NLP Preprocessing Pipeline**  
2. **Q2: Named Entity Recognition with spaCy**  
3. **Q3: Scaled Dot‑Product Attention**  
4. **Q4: Sentiment Analysis using HuggingFace Transformers**  

Each task includes:  
- A self‑contained Python script or notebook.  
- A clear README section with instructions.  
- Example input, expected output, and short answers to conceptual questions.  

---

## 🗂 Project Structure  
```
.
├── Q1_NLP_Preprocessing/
│   ├── preprocess.py       # tokenization, stopword removal, stemming
│   └── README.md           # task description & how to run
│
├── Q2_NER_spaCy/
│   ├── ner_spacy.py        # spaCy pipeline for NER extraction
│   └── README.md           # task description & how to run
│
├── Q3_Scaled_DotProduct_Attention/
│   ├── attention.py        # implement & test scaled dot-product attention
│   └── README.md           # task description & how to run
│
└── Q4_Sentiment_Transformers/
    ├── sentiment.py        # HuggingFace pipeline example
    └── README.md           # task description & how to run
```

---

## ⚙️ Requirements & Setup  

1. **Clone the repo**  
   ```bash
   git clone https://github.com/your‑username/your‑repo.git
   cd your‑repo
   ```
2. **Install dependencies**  
   ```bash
   pip install nltk spacy transformers numpy sklearn
   python -m spacy download en_core_web_sm
   ```
3. **Run each module**  
   - Navigate into one of `Q1_…`, `Q2_…`, etc.  
   - Execute the script:  
     ```bash
     python preprocess.py     # for Q1
     python ner_spacy.py      # for Q2
     python attention.py      # for Q3
     python sentiment.py      # for Q4
     ```

---

## 📋 Task Summaries  

### Q1: NLP Preprocessing Pipeline  
- **Steps:**  
  1. Tokenize a sample sentence.  
  2. Remove English stopwords.  
  3. Apply Porter stemming.  
- **Short Answers:**  
  1. Stemming vs. Lemmatization (e.g. “running”→“run” via stemmer vs. lemmas).  
  2. When stopwords help (topic modeling) vs. hurt (sentiment flip “not”).  

### Q2: Named Entity Recognition  
- **Steps:**  
  1. Load `en_core_web_sm`.  
  2. Extract entities, labels, and character spans.  
- **Short Answers:**  
  1. NER (semantic spans) vs. POS tagging (syntactic labels).  
  2. Applications: financial news extraction, search‑engine entity linking.  

### Q3: Scaled Dot‑Product Attention  
- **Implementation:**  
  1. Compute Q·Kᵀ  
  2. Scale by √d  
  3. Softmax → attention weights  
  4. Multiply weights by V  
- **Short Answers:**  
  1. √d prevents softmax saturation in high‑dim.  
  2. Self‑attention models long‑range word dependencies.  

### Q4: Sentiment Analysis with Transformers  
- **Steps:**  
  1. Load HuggingFace `pipeline("sentiment-analysis")`.  
  2. Classify example sentence.  
- **Short Answers:**  
  1. BERT = encoder‑only, GPT = decoder‑only.  
  2. Pre‑trained models save compute, data, and provide strong baselines.  

---
