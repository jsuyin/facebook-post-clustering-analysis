# 📊 Facebook Post Clustering Analysis

**Author:** Justin Mundell  

---

## Overview
This project explores user engagement patterns on Facebook posts using unsupervised learning techniques. The goal is to identify natural groupings in post performance and determine whether engagement metrics align with post types such as photos, videos, links, and status updates. 

---

## Objectives
- Identify clusters in Facebook engagement data  
- Determine the optimal number of clusters  
- Evaluate whether clusters correspond to post types  

---

## Dataset
- ~7,000 Facebook posts  
- Sourced from Facebook API (Thai retail pages)  
- Features include:
  - reactions, comments, shares  
  - likes and emoji reactions (love, wow, haha, etc.) 

---

## Methods
- Exploratory Data Analysis (EDA)  
- Principal Component Analysis (PCA)  
- K-Means Clustering  
- Hierarchical Clustering (complete, average, single linkage)  
- Cluster validation:
  - Silhouette score  
  - Gap statistic  

---

## Results

- PCA:
  - First 2 components explain ~57% of variance  
  - First 5 components explain ~86% of variance  

- K-Means:
  - Best clustering found at **K=2** (highest silhouette ~0.82)  
  - K=4 aligns with actual post types but shows overlap  

- Hierarchical Clustering:
  - Best silhouette score ~0.92 (average linkage)  
  - Also suggests **2 main clusters**  

---

## Key Insights

- Strong clustering into **2 dominant groups (photos vs videos)**  
- Engagement metrics (likes, reactions) are highly correlated  
- Data imbalance (more photos/videos) impacts clustering quality  
- PCA effectively reduced dimensionality while preserving structure  

---

## Files
- `Math 4323 Project.pdf` – Full analysis and code  

---

## Notes
Clustering results were influenced by dataset imbalance and limited representation of some post types (e.g., links and status updates), which may affect the ability to recover all expected clusters. 
