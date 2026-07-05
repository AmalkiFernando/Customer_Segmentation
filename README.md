# 🤖 Customer Segmentation using K-Means Clustering

![Python](https://img.shields.io/badge/Python-3.10+-blue?logo=python&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-1.x-orange?logo=scikitlearn&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-2.x-150458?logo=pandas&logoColor=white)
![Status](https://img.shields.io/badge/Status-Complete-brightgreen)
---

## 📌 Project Overview

This project applies **K-Means Clustering**, an unsupervised machine learning algorithm, to segment mall customers into meaningful groups based on their purchasing behavior. By analyzing **Age**, **Annual Income**, and **Spending Score**, the project identifies customer segments that can support targeted marketing strategies and business decision-making.

The optimal number of clusters was determined using both the **Elbow Method** and **Silhouette Score**. Each cluster was profiled and interpreted to provide actionable marketing recommendations.

---

## 📂 Dataset Information

| Property | Details |
|-----------|---------|
| Dataset | Mall Customers Dataset |
| Records | 200 Customers |
| Features | 5 |
| Missing Values | None |

## Dataset Features

| Feature | Description |
|----------|-------------|
| CustomerID | Unique customer identifier (removed before clustering) |
| Gender | Label encoded during preprocessing |
| Age | Customer age |
| Annual Income (k$) | Annual income in thousand dollars |
| Spending Score (1-100) | Spending behavior score assigned by the mall |

---

## ⚙️ Technologies Used

| Technology | Purpose |
|------------|---------|
| Python | Programming Language |
| Pandas | Data manipulation |
| NumPy | Numerical computation |
| Matplotlib | Data visualization |
| Seaborn | Statistical visualization |
| Scikit-learn | Machine Learning |
| Joblib | Save & Load trained models |

---
## 🤖 Machine Learning Pipeline

### K-Means Clustering

**Pipeline:**
1. Load the **Mall Customers** dataset into a Pandas DataFrame.
2. Encode the **Gender** column using Label Encoding.
3. Remove `CustomerID` and `Encoded_Gender`before clustering.
4. Select the clustering features:- `Age`, `Annual Income (k$)`,`Spending Score (1-100)`
5. Standardize the selected features using **StandardScaler**.
6. Determine the optimal number of clusters using **Elbow Method** and **Silhouette Score** (k = 2 to 10)
7. Train the model using **optimal k = 6**
8. Profile each cluster using average **Age**, **Annual Income**, **Spending Score**, and **Customer Count**.
9. Assign meaningful names and define marketing recommendations.

---

## 📈 Choosing the Optimal k

The optimal number of clusters was evaluated using both the **Elbow Method** and **Silhouette Score**.

| K | Inertia (WCSS) | Silhouette Score |
|---|---------------:|-----------------:|
| 2 | 389.386189 | 0.335472 |
| 3 | 295.212246 | 0.357793 |
| 4 | 205.225147 | 0.403958 |
| 5 | 168.247580 | 0.416643 |
| **6** | **133.868421** | **0.428417** ✅ |
| 7 | 117.011555 | 0.417232 |
| 8 | 103.873292 | 0.408207 |
| 9 | 93.092891  | 0.417693 |
| 10 | 82.385154 | 0.406554 |

**K = 6** clusters were selected based on the Elbow Method and Silhouette Score.
---

## 📊 Cluster Summary

| Cluster | Segment | Customer Count | Average Age | Average Income | Average Spending |
|---------|----------------------------|---------------:|------------:|---------------:|-----------------:|
| 0 | Older Average Spenders | 45 | 56.33 | 54.27 | 49.07 |
| 1 | Young Average Spenders | 39 | 26.79 | 57.10 | 48.13 |
| 2 | High Income Low Spenders | 33 | 41.94 | 88.94 | 16.97 |
| 3 | High Income High Spenders | 39 | 32.69 | 86.54 | 82.13 |
| 4 | Young High Spenders | 23 | 25.00 | 25.26 | 77.61 |
| 5 | Low Income Low Spenders | 21 | 45.52 | 26.29 | 19.38 |

---

## 💡 Marketing Recommendations

**High Income High Spenders** – VIP membership programs, premium product recommendations, exclusive rewards, and loyalty programs.

**High Income Low Spenders** – Personalized promotions, product bundles, and loyalty incentives to encourage increased purchases.

**Young High Spenders** – Trend-focused products, student discounts, influencer collaborations, and social media marketing campaigns.

**Young Average Spenders** – Personalized recommendations, seasonal promotions, and customer engagement campaigns.

**Older Average Spenders** – Repeat purchase incentives, personalized services, and family-oriented promotions.

**Low Income Low Spenders** – Budget-friendly products, discount campaigns, and coupon offers.

---

## 📁 Project Structure

```
Customer-Segmentation-KMeans/
│
├── Analysis_Model.ipynb            # note book
├── Mall_Customers.csv              # reference dataset
├── Mall_Customers_Clustered.csv    # dataset with cluster labels
├── KMeans_Model.pkl                # K-Means model
├── StandardScaler.pkl              # StandardScaler
├── requirements.txt                # project dependencies
└── README.md
```

---

## 👩‍💻 Author

**Amalki Fernando**
BSc (Hons) in IT Specialising in Artificial Intelligence
[SLIIT] — [2026]
