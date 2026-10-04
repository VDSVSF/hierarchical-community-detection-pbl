# Inferring Latent Graph Communities via Hierarchical Clustering and Supervised User Profile Attribution

**Authors:** Vedant Chopkar, Vincy Jain  
**Affiliation:** Department of Electronics and Communication Engineering, Bharati Vidyapeeth (DU) College of Engineering, Pune  

---

## 📌 Project Overview
This repository contains the complete experimental code, dataset processing pipeline, and paper for the Machine Learning Problem-Based Learning (PBL) project.

The project implements a two-stage learning framework:
1. **Unsupervised Community Detection:** Spectral graph embedding combined with Ward-linkage Agglomerative Hierarchical Clustering to detect modular communities on graph topology, evaluated using Newman's Modularity ($Q$).
2. **Supervised Profile Attribution:** An XGBoost multi-class classifier trained on TF-IDF weighted user profile feature tags to predict community membership without topological adjacency at inference time.

---

## 📊 Key Results
- **Dataset:** Stanford SNAP Twitch Social Network (ENGB subset, $N = 1,500$ nodes)
- **Detected Communities:** $k^* = 3$ (Newman's Modularity $Q = 0.3642$)
  - Community 0: 688 users
  - Community 1: 451 users
  - Community 2: 361 users
- **Classification Performance:**
  - **Overall Accuracy:** 63.73% (vs. 33.33% uniform random baseline)
  - **Macro-Averaged F1-Score:** 0.6068

---

## 📁 Repository Structure
- `PBL_Community_Detection_Paper_Vedant_Vincy.pdf`: Complete paper formatted in the Springer Nature (`sn-jnl`) template.
- `community_detection_pipeline.ipynb`: End-to-end Python pipeline (data download, spectral decomposition, hierarchical clustering, and XGBoost training).
- `sn-article.tex`: Full LaTeX source file.

---

## 🚀 Execution Instructions
1. Open Google Colab.
2. Upload and run `community_detection_pipeline.ipynb`.
3. The dataset is automatically retrieved and extracted directly from the Stanford SNAP repository.# hierarchical-community-detection-pbl
