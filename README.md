# Mall Customer Segmentation using K-Means Clustering

A data science project focused on customer segmentation using the K-Means clustering algorithm. This project demonstrates practical applications of **Unsupervised Learning** to group mall customers based on their annual income and spending behavior.

---

## 📌 Project Overview
The goal of this project is to analyze customer data and divide them into distinct groups (clusters) to help the marketing team design targeted and efficient business strategies.

## 🛠️ Data & Feature Engineering Decisions
During the development process, critical engineering choices were made regarding feature selection:
* **Gender & Age:** Initially explored using One-Hot Encoding and 3D plotting. However, they added unnecessary noise and created heavily overlapping clusters. They were dropped to maintain clear separation and realistic business logic.
* **Final Features Used:** `Annual Income (k$)` and `Spending Score (1-100)`.

## 📊 Methodology & Optimization
1. **The Elbow Method:** Used to find the optimal number of clusters ($K$). The curve clearly indicated a sharp elbow point at **$K = 5$**.
2. **Model Training:** Built using `scikit-learn`'s `KMeans` with `init='k-means++'` and `random_state=42` for stable and reproducible results.

## 📈 Final Segmentation Result
The model successfully partitioned the customers into **5 well-defined segments** with distinct centroids:

* **Cluster 1:** Low Income, Low Spend (Sensible)
* **Cluster 2:** Medium Income, Medium Spend (Standard)
* **Cluster 3:** High Income, High Spend (VIP)
* **Cluster 4:** Low Income, High Spend (Careless)
* **Cluster 5:** High Income, Low Spend (Careful)

*(Tip: You can insert your final 2D cluster image here by uploading it to your repo and using: `![Final Clusters](image_name.png)`)*

---

## 🚀 Frameworks Used
* Python 3
* Pandas & NumPy
* Scikit-Learn
* Matplotlib & Seaborn
