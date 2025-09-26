# Text Clustering using NMF and LSA 

This project is focuses on **feature extraction and text clustering using Nonnegative Matrix Factorization (NMF) and Latent Semantic Analysis (LSA)**.

## 📌 Introduction
Text clustering is one of the main challenges in modern data mining. Text data are usually high-dimensional and sparse, leading to the **curse of dimensionality**. This project introduces a method for dimension reduction and stable feature representation by applying NMF-based feature fusion and **Spherical K-Means** clustering.

## ⚙️ Features
- **Tokenization, stopword removal, stemming, TF-IDF**
- **NMF with NNDSVD initialization**
- Feature space construction by merging word vectors
- Optional **LSA** for further dimensionality reduction
- **Spherical K-Means** for document clustering
- Evaluation metrics:
  - **Purity**
  - **NMI (Normalized Mutual Information)**
  - **ARI (Adjusted Rand Index)**
- Comparison with other approaches:
  - K-Means
  - K-Means++
  - LSA + K-Means
  - Spectral Clustering + PSO
  - Genetic Algorithm + K-Means

## 🛠️ Requirements
```bash
Python 3.8+
numpy
scipy
pandas
scikit-learn
matplotlib
nltk
```

## 🚀 How to Run
```bash
git clone https://github.com/username/text-clustering-nmf-lsa.git
cd text-clustering-nmf-lsa
pip install -r requirements.txt
jupyter notebook FinalProjectMainPart.ipynb
jupyter notebook FinalProjectComparePart.ipynb
```

## 📊 Datasets
- **20 Newsgroups**
- **AG News**
- **BBC News & BBC Sports**
- **DMOZ**
- **SMS Spam Collection**

## 📈 Results
- The proposed method (NMF-FR) achieved **more stable** and in many cases **more accurate** clustering results compared to baseline methods.
- **SVD-based initialization** improved stability over random initialization.
- Significant improvements observed in **Purity, NMI, and ARI** metrics across multiple datasets.

## 📚 References
1. Ali Hassani (2020). *Text Mining using Nonnegative Matrix Factorization and Latent Semantic Analysis*
2. [Spectral Clustering - Wikipedia](https://en.wikipedia.org/wiki/Spectral_clustering)
3. [Wilcoxon Signed-Rank Test - Wikipedia](https://en.wikipedia.org/wiki/Wilcoxon_signed-rank_test)
4. [Optimal dimensions for LSA](https://codingtechroom.com/question/optimal-dimensions-latent-semantic-analysis)
5. [NMF optimal number of components in sklearn](https://stackoverflow.com/questions/67473597/how-to-select-optimal-number-of-components-for-nmf-in-python-sklearn)
