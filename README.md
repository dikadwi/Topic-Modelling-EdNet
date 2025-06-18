
# 📚 Topic Modeling for Constructing Learning Profiles Using LDA and Coherence Evaluation

This repository contains source code, data preprocessing scripts, and experimental notebooks used in the study:

> **"Topic Modeling for Constructing Learning Profiles Using LDA and Coherence Evaluation"**
> > *Andika Dwi Arko*, *Muhamad Yusril Helmi Setyawan* , *Roni Andarsyah*

## 🧠 Overview

Penelitian ini mengembangkan pendekatan untuk membentuk **profil pembelajaran berbasis topik** dari data interaksi siswa skala besar menggunakan algoritma **Latent Dirichlet Allocation (LDA)**. Dataset yang digunakan adalah **EdNet-KT1**, yang berisi interaksi siswa dengan pertanyaan berdasarkan tag semantik. Setiap pertanyaan dikonversi menjadi pseudotext, dimodelkan menjadi 20 topik, dan dihubungkan dengan akurasi siswa pada setiap topik untuk membentuk matriks kinerja siswa.

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
│   ├── PyLDAvis.png
│   ├── Heatmap_Learning_Profile.png
│   ├── Radar_chart.png
│   ├── PCA_Clustering.png
│   ├── Top10_Recommended_Topic.png
│   ├── line_chart.png
│   └── comparison_coherence_lda.png
└── README.md
└── LICENSE
└── requirements.txt
```

## 📊 Dataset

- **EdNet-KT1**: A large-scale dataset of 131M+ interactions from ~784K students.
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
  Email: [adwiarko@gmail.com]

```
