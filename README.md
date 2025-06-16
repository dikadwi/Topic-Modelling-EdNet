
# 📚 Topic Modeling for Constructing Learning Profiles Using LDA and Coherence Evaluation

This repository contains source code, data preprocessing scripts, and experimental notebooks used in the study:

> **"Topic Modeling for Constructing Learning Profiles Using LDA and Coherence Evaluation"**  
> Submitted to *JUTI: Jurnal Ilmiah Teknologi Informasi*

## 🧠 Overview

This project proposes a semantic-based learning profiling approach by applying **Latent Dirichlet Allocation (LDA)** to the **EdNet-KT1** dataset. The aim is to model topics from educational interaction data and construct student learning profiles based on topic-wise performance.

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
│   ├── 1_preprocessing_ednet.ipynb
│   ├── 2_generate_pseudotext.ipynb
│   ├── 3_topic_modeling_lda.ipynb
│   ├── 4_student_accuracy_matrix.ipynb
│   ├── 5_clustering_analysis.ipynb
│   └── 6_topic_recommendation.ipynb
├── data/
│   ├── EdNet-KT1/
│   ├── interaksi_soal_gabungan.csv
│   ├── question.csv
│   ├── soal_pseudo_text.csv
│   ├── soal_topik.csv
│   ├── representasi_topik_siswa.csv
│   └── rekomendasi_pembelajaran_adaptif.csv
├── figures/
│   ├── fig_1_methodology_flowchart.png
│   ├── fig_3_pyldavis.png
│   ├── fig_4_heatmap_accuracy.png
│   ├── fig_5_radar_chart.png
│   ├── fig_6_pca_clustering.png
│   ├── fig_7_bar_recommendation.png
│   └── fig_8_coherence_score_plot.png
└── README.md
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

## 🛠️ Technologies

- Python 3.9
- Gensim
- Scikit-learn
- Pandas, Numpy, Matplotlib, Seaborn
- NLTK
- PyLDAvis

## 📜 Citation

If you use this code or data, please cite the associated paper (once published).  

```bibtex
@article{arko2025lda,
  title={Topic Modeling for Constructing Learning Profiles Using LDA and Coherence Evaluation},
  author={Andika Dwi Arko and Muhamad Yusril Helmi Setyawan},
  journal={JUTI: Jurnal Ilmiah Teknologi Informasi},
  year={2025}
}
```

## 📬 Contact

- **Andika Dwi Arko**  
  Email: [adwiarko@gmail.com](mailto:adwiarko@gmail.com)
