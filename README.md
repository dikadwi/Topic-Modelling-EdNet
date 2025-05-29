# 📘 Topic Modeling for Learning Profile Extraction using LDA on EdNet-KT1 Dataset

This repository contains source code, data subsets, and visualization notebooks related to the research:

> **"Topic Modeling to Form Learning Profiles Using LDA and Coherence Evaluation"**  
> *Andika Dwi Arko*, *Muhamad Yusril Helmi Setyawan*  
> University of Logistics and International Business  
> Submitted to: JUTI – Scientific Journal of Information Technology

---

## 🔍 Overview

This project explores how **Latent Dirichlet Allocation (LDA)** can be used to model question topics and generate **semantic learning profiles** for students using large-scale data from the **EdNet-KT1** dataset. Students’ interactions with tagged questions are transformed into pseudotexts, clustered by dominant topic, and used to calculate **topic-wise accuracy**. These representations form the basis for **student segmentation** and **adaptive learning recommendations**.

---

## 🧪 Key Features

- Semantic topic extraction with **LDA** (via Gensim)
- Coherence evaluation (c_v metric: **0.6688** with 20 topics)
- Topic-wise student accuracy matrix (user × topic)
- Visual analytics: **heatmap**, **radar chart**, **line plot**, **PCA**
- Clustering of students using **K-Means**
- Topic recommendations based on accuracy thresholds

---



