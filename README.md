# 🧠 Mental Health Conversations Topic Modeling

This project explores topic modeling on mental health conversation data using Latent Dirichlet Allocation (LDA) and BERTopic.
The dataset is sourced from **Psychika Dataset**, which contains Indonesian conversational text related to psychology and mental health.

## 📂 Dataset

`Source:` [Psychika Dataset Kaggle](https://www.kaggle.com/datasets/xmaulana/psychikadataset-7b/data)

Contains Indonesian conversational text regarding **mental health, psychology, and counseling.**

## 🔍 Methods

I applied two topic modeling approaches:

## 1. Latent Dirichlet Allocation (LDA)

**Definition**  
LDA is a classical probabilistic method for topic modeling.  

**How It Works**  
- A document is considered a mixture of several topics.  
- Each topic is represented as a distribution of words.  
- LDA applies the *Dirichlet distribution* to model topic probabilities within documents and word probabilities within topics.  

**Strengths**  
- Simple and widely adopted.  
- Effective for many traditional text-mining tasks.  

**Limitations**  
- Sensitive to parameter tuning.  
- Struggles to capture semantic context (e.g., synonyms may not be grouped together).  

---

## 2. BERTopic

**Definition**  
BERTopic is a modern topic modeling technique that leverages **transformer-based embeddings** (e.g., BERT, Sentence-BERT).  

**How It Works**  
1. Generate text representations using transformer embeddings.  
2. Cluster documents using algorithms such as **HDBSCAN**.  
3. Extract representative keywords for each topic using **c-TF-IDF**.  

**Strengths**  
- Better captures semantic meaning.  
- Produces more coherent and interpretable topics.  
- Flexible: works with different language models.  

**Limitations**  
- Computationally heavier.  
- Performance depends on the quality of embeddings.

---
## 🚀 Installation
Clone this repository and install dependencies:
```bash
git clone https://github.com/MuthiahAinun/topic-modeling-mental-health-convo.git
cd topic-modeling-mental-health-convo
pip install -r requirements.txt
```
---
## 📊 Results
### LDA
**Topic 1: Uncertainty & Existential Questions**

![][topic1.png]

**Key terms:** people, maybe, know, true, feel, ask, act/do, say, more, make/do

**Interpretation:** This topic revolves around doubt, questioning truth, and seeking validation from others. It suggests conversations filled with uncertainty and reflection about what is “true” or “right.”

---
**Topic 2: Seeking Help & Anxiety Therapy**

![][topic2.png]

**Key terms:** people, help, therapy, own, anxiety, feel, maybe, treatment, healthy, several

**Interpretation:** Clearly related to seeking support and therapy for anxiety and mental health. It emphasizes the role of both professional treatment and social support in coping with psychological distress.

---
**Topic 3: Family & Parenting**

![][topic3.png]

**Key terms:** child, people, mother, parent/elder, act/do, father, family, know, how, maybe

**Interpretation:** This topic is strongly tied to family dynamics, parenting roles, and relationships between parents and children. It indicates discussions about responsibilities, care, and challenges within family life.

---
**Topic 4: Self-Reflection & Personal Thoughts**

![][topic4.png]

**Key terms:** think, self, feel, people, act/do, more, alone/self, day, good, maybe

**Interpretation:** This topic highlights introspection, personal feelings, and self-talk. It reflects inner struggles, self-evaluation, and how individuals perceive their daily lives and well-being.

---
**Topic 5: Relationships & Identity**

![][topic5.png]

**Key terms:** relationship, people, own, feel, self, maybe, together/same, act/do, good, many

**Interpretation:** This topic centers on social connections, belonging, identity, and self-worth within relationships. It captures the balance between individuality and togetherness in social or intimate contexts.

---
**🎯 Overall Conclusion**

The five topics map onto key dimensions of mental health discourse:

1. Uncertainty & existential questioning
2. Support systems & therapy for anxiety
3. Family and parenting dynamics
4. Self-reflection and personal thought processes
5. Relationships, belonging, and identity

---
### BERTopic

#### 🌐 Topic Modeling Insights on Mental Health Conversations

![][newplot.png]

## 🧩 Topic 0 – Therapy & Treatment  
**Keywords:** *terap, tepat, latih, awat, bagaimana*  
Focuses on **therapy practices and best approaches** — from training to treatment methods.  

---

## 💊 Topic 1 – Depression & Medical Symptoms  
**Keywords:** *depresi, obat, cemas, gejala, dokter*  
Covers discussions around **depression, medication, anxiety, and medical symptoms**.  

---

## 🛌 Topic 2 – Counseling & Sleep Issues  
**Keywords:** *konseling, milik, masalah, insomnia, kanker*  
Highlights the role of **counseling** in addressing **personal struggles, insomnia, and even serious health conditions**.  

---

## 😌 Topic 3 – Emotions & Normalization  
**Keywords:** *menang, terapi, normal, emosi, lama*  
Explores **emotional regulation, therapy sessions, and the pursuit of normalcy**.  

---

## 👩‍🎓 Topic 4 – Adolescents & Social Support  
**Keywords:** *remaja, depresi, teman, minggu, kelas*  
Centers on **teenagers, peer support, school activities**, and the challenges of depression among youth.  

---

## 🧠 Topic 5 – Mental Health & Support Systems  
**Keywords:** *obat, mental, sehat, dukung, ingat*  
Emphasizes the importance of **mental health care, medical treatment, and supportive environments**.  

---

## 📚 Topic 6 – Stress & School Life  
**Keywords:** *putri, stres, khawatir, sekolah, konyol*  
Addresses **school-related stress, worries, and emotional struggles**, especially among young women.  

---

## 📞 Topic 7 – Therapy Process & Online Counseling  
**Keywords:** *terap, proses, klien, telepon, sesi*  
Focuses on **formal therapy processes** including **remote/phone counseling sessions**.  

---

## 🌑 Topic 8 – Loneliness & Emptiness  
**Keywords:** *sendiri, diri, kosong, rasa, kata*  
Captures **feelings of isolation, emptiness, and deep self-reflection**.  

---

## ⚠️ Topic 9 – Negative Thoughts & Suicidal Ideation  
**Keywords:** *harga, betapa, bunuh, pikir, asa*  
Deals with **suicidal thoughts, hopelessness, and reflections on self-worth**.  

---

# 📝 Key Takeaways  
The conversations largely revolve around **core mental health issues**:  

- **Therapy & counseling** → *Topics 0, 2, 3, 7*  
- **Depression & medication** → *Topics 1, 5*  
- **Adolescents & school-related stress** → *Topics 4, 6*  
- **Loneliness & suicidal thoughts** → *Topics 8, 9*  

👉 Together, these topics reveal a **spectrum of mental health struggles** ranging from **clinical treatments** to **personal emotions and social contexts**.

---
## 🔑 Final Conclusion

This project demonstrates how **topic modeling** (via **LDA** and **BERTopic**) can uncover meaningful structures within mental health conversations.  

- **LDA** reveals broad, abstract themes such as uncertainty, therapy, family roles, self-reflection, and identity in relationships.  
- **BERTopic**, with its embedding-based approach, provides more **fine-grained and context-aware insights**, surfacing topics like therapy practices, depression and medication, adolescent stress, online counseling, loneliness, and suicidal ideation.  

🧠 **Overall Insight:**  
Mental health discourse spans across both **clinical aspects** (therapy, medication, counseling) and **personal-emotional struggles** (identity, stress, loneliness, suicidal thoughts).  
These findings highlight the importance of combining **professional treatment**, **social support**, and **personal reflection** in addressing mental health challenges.

---
