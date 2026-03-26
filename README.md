# Hierarchical Text Classification using Kernel Methods for NLP

This repository contains the implementation and research findings of my **Master's Thesis at AIMS Senegal**. The project focuses on improving the reliability of hierarchical classification for scientific publications within the **Web of Science (WOS)** taxonomy.

##  Key Contributions

* **14x Reliability Leap:** Improved Full-Path Accuracy (exact match from root to leaf) from 44 to 775 documents in the test set.
* **Kernel Reactivation:** Demonstrated that **BERT dense embeddings** "reactivate" the **RBF and Polynomial kernels**, which typically fail or remain unstable with sparse statistical vectors (TF-IDF).
* **Green AI & Efficiency:** Developed a hybrid BERT-SVM architecture that is **70x faster** to train than Random Forest baselines while maintaining high precision.
* **Logical Rigor:** Guaranteed a **0.00% hierarchical violation rate** using the Local Classifier per Parent Node (LCPN) architecture.

## Technologies & Methodology

### NLP & Vectorization
* **Statistical Approach:** TF-IDF (Term Frequency-Inverse Document Frequency) used as a baseline for sparse representation.
* **Contextual Approach:** BERT (Bidirectional Encoder Representations from Transformers) via HuggingFace for dense semantic embeddings.

### Machine Learning Models
* **Baselines:** Random Forest (RF) and Linear SVC.
* **Core Models:** Support Vector Machines (**SVM**) with multiple kernels (**Linear, RBF, and Polynomial**) using Scikit-Learn.

### Architecture
* **LCPN (Local Classifier per Parent Node):** A specialized hierarchical strategy that decomposes the classification task into local, manageable nodes to handle class imbalance effectively.


## 📂 Repository Structure

* **notebooks/**
    * 01_Baseline_TFIDF_SVM_RF.ipynb`: Comparison of statistical methods and traditional machine learning.
    * 02_Advanced_BERT_SVM_Hybrid.ipynb`: Implementation of BERT embeddings and non-linear kernel reactivation.
* **docs/**
    * Master_Thesis_Fatou_Kine.pdf: The full academic document defended at AIMS Senegal.
* **requirements.txt**: List of dependencies (transformers, scikit-learn, pandas, etc.).

## 🎓 Author

**Fatou Kiné Touré**
*Junior Data Scientist & AI Consultant | AIMS Senegal Alumni.
