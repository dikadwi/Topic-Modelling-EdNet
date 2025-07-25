
# 📚 Topic Modeling for Constructing Learning Profiles Using LDA and Coherence Evaluation

This repository contains source code, data preprocessing scripts, and experimental notebooks used in the study:

> **"Topic Modeling for Constructing Learning Profiles Using LDA and Coherence Evaluation"**
> > *Andika Dwi Arko*, *Muhamad Yusril Helmi Setyawan* , *Roni Andarsyah*
> > *https://doi.org/10.12962/j24068535.v23i2.a1301*

## 🧠 Overview

This study develops an approach to form **topic-based learning profiles** from large-scale student interaction data using the **Latent Dirichlet Allocation (LDA)** algorithm. The dataset used is **EdNet-KT1**, which contains student interactions with questions based on semantic tags. Each question is converted into pseudotext, modeled into 20 topics, and linked to student accuracy on each topic to form a student performance matrix.

## 🔍 Objectives

- Generate pseudotext from semantic tags of questions.
- Train an LDA model and evaluate its semantic quality using **coherence score (c_v)**.
- Map questions to dominant topics and calculate student accuracy per topic.
- Cluster students using **K-Means** and visualize their performance using **PCA**, **heatmaps**, and **radar charts**.
- Recommend topics for improvement based on student-topic mastery.

## 📁 Folder Structure

```
.
├── notebook/
│   ├── Analisis_LDA_Siswa.ipynb
├── file_output/
│   ├── 1.combined_question_interaction.csv
│   ├── 2.pseudotexts_question.csv
│   ├── 3.topic_question.csv
│   ├── 4.student_topic_representation.csv
│   ├── 5.student_grade_matrix_topic.csv
│   ├── 6.user_topic_matrix.csv
|   └── 7.student_topic_cluster.csv
├── Visualization/
│   ├── Heatmap_Learning_Profile.png
│   ├── PCA_Clustering.png
│   ├── PyLDAvis.png
│   ├── PyLDAvizlda_visualisasi.html
│   ├── Radar_chart.png
│   ├── Top10_Recommended_Topic.png
│   ├── comparison_coherence_lda.png
│   └── line_chart.png
└── README.md
└── LICENSE
└── requirements.txt
```

## 📊 Dataset

- **EdNet-KT1**: A large-scale dataset of 131M+ interactions from ~784K students.
- **question**: file provides metadata for each question used in the EdNet-KT1 dataset. It contains 7 columns, each describing key attributes of a *question_id, bundle_id, explanation_id, correct_answer, part, tags, deployed_at*.
- Source: [EdNet GitHub](https://github.com/riiid/ednet)
- For this study, a **subset of 1,000 log files** was used (≈154K rows) for computational efficiency and topic diversity.

## 🧪 Main Results

| Component                    | Description                                                                 |
|-----------------------------|-----------------------------------------------------------------------------|
| **LDA Topics**              | 20 topics with coherence score of **0.6688**                               |
| **Student Accuracy Matrix** | 66% of students mastered more than five topics                            |
| **Clustering (K-Means)**    | 4 clusters: high, low, average, and inconsistent performers                |
| **Visualization Tools**     | PyLDAvis, heatmaps, radar charts, PCA                                      |
| **Adaptive Recommendations**| Topics with accuracy < 0.5 and interaction > 10 identified as weak areas   |

## 🛠️ Technologies / requirements
- Using Google Colab
- Python 3.9
- Gensim
- Scikit-learn
- Pandas, Numpy, Matplotlib, Seaborn
- NLTK
- PyLDAvis

## 📬 Contact

**Andika Dwi Arko**  
  Email: adwiarko@gmail.com

## 📜 License
This project is shared under a custom MIT-style license with restrictions. 
Usage is free for academic/non-commercial purposes with attribution. 
Modification or redistribution requires permission from the author (adwiarko@gmail.com).

