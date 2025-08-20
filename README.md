# 🧠 Mental Health Conversations Topic Modeling

This project explores topic modeling on mental health conversation data using Latent Dirichlet Allocation (LDA) and BERTopic.
The dataset is sourced from Psychika Dataset
, which contains Indonesian conversational text related to psychology and mental health.

## 📂 Dataset

`Source:` (Psychika Dataset (Kaggle))[https://www.kaggle.com/datasets/xmaulana/psychikadataset-7b/data]

Contains Indonesian conversational text regarding **mental health, psychology, and counseling.**

## 🔍 Methods

I applied two topic modeling approaches:

**1. Latent Dirichlet Allocation (LDA)**

- Preprocessing with tokenization, stopwords removal, and lemmatization.
- Bag-of-Words representation via CountVectorizer.
- Extracted 10 top keywords per topic.

**2. BERTopic**

- Transformer-based topic modeling.
- Used embeddings from a pre-trained Indonesian language model.
- More coherent and semantically meaningful topics compared to LDA.

Visualized with interactive BERTopic visualization tools.
## 🚀 Installation
Clone this repository and install dependencies:
```bash
git clone https://github.com/username/lda-mental-health-conversations.git
cd lda-mental-health-conversations
pip install -r requirements.txt
```
---
## 📊 Results
### LDA
**Topic 1: Uncertainty & Existential Questions**
(Topic 1)[!topic1.png]


**Key terms:** people, maybe, know, true, feel, ask, act/do, say, more, make/do

**Interpretation:** This topic revolves around doubt, questioning truth, and seeking validation from others. It suggests conversations filled with uncertainty and reflection about what is “true” or “right.”

---
**Topic 2: Seeking Help & Anxiety Therapy**

**Key terms:** people, help, therapy, own, anxiety, feel, maybe, treatment, healthy, several

**Interpretation:** Clearly related to seeking support and therapy for anxiety and mental health. It emphasizes the role of both professional treatment and social support in coping with psychological distress.
