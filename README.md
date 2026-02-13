# Behavioral Clustering Analysis

**Exploring K-Means and Hierarchical Clustering in Multi-Dimensional Data**

## Overview

This project investigates how clustering algorithms identify structure in behavioral data.

Instead of applying clustering as a black box, the goal was to:

* Design a synthetic multi-feature dataset
* Understand the impact of feature scaling
* Compare K-Means and Hierarchical Clustering
* Evaluate cluster quality quantitatively

The focus is on *geometric intuition and model assumptions*, not just implementation.

---

## Dataset

A synthetic behavioral dataset was created with five features:

* Risk Tolerance
* Decision Speed
* Information Seeking
* Consistency
* Reward Sensitivity

The dataset embeds three latent behavioral archetypes to test whether clustering algorithms can recover structured patterns.

---

## Methods

* **Standardization (StandardScaler)** to ensure fair distance computation
* **K-Means Clustering (K=3)** using inertia and the elbow method
* **Agglomerative Hierarchical Clustering (Ward linkage)**
* **Silhouette Score** for quantitative evaluation
* Cross-tab analysis to compare algorithm agreement

---

## Results

* Both algorithms identified three meaningful behavioral groups.
* Near-identical cluster assignments across methods.
* Silhouette score ≈ **0.51**, indicating moderate-to-strong structure.
* Strong separation for extreme profiles; moderate overlap for transitional group.

These results show that when structure is variance-driven and compact, different clustering methods converge to similar solutions.

---

## 🔎 Key Takeaways

* Clustering outcomes depend heavily on feature scaling and distance geometry.
* K-Means and Ward linkage behave similarly under spherical assumptions.
* Evaluation metrics are essential — visual inspection alone is insufficient.
* Unsupervised learning reveals structure under assumptions, not absolute truth.

---

## Tech Stack

Python • Pandas • NumPy • Matplotlib • Seaborn • Scikit-learn

---

## Skills Demonstrated

* Unsupervised Learning
* Clustering Evaluation
* Model Comparison
* Data Preprocessing
* Analytical Interpretation
* Clear Technical Communication
