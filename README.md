# 🛍️ Customer Segmentation using K-Means Clustering

![Python](https://img.shields.io/badge/Python-3.10+-blue?logo=python&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-1.x-orange?logo=scikitlearn&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-2.x-150458?logo=pandas&logoColor=white)
![Status](https://img.shields.io/badge/Status-Complete-brightgreen)

---

## 📌 Project Overview

This project applies **K-Means Clustering**, an unsupervised machine learning algorithm, to segment mall customers into meaningful groups based on their purchasing behavior. By analyzing **Age**, **Annual Income**, and **Spending Score**, the project identifies customer segments that can support targeted marketing strategies and business decision-making.

The optimal number of clusters was determined using both the **Elbow Method** and **Silhouette Score**. Each cluster was profiled and interpreted to provide actionable marketing recommendations.

---

## 🎯 Objectives

- Perform exploratory data analysis (EDA)
- Clean and preprocess customer data
- Encode categorical features
- Scale numerical features
- Determine the optimal number of clusters
- Apply K-Means clustering
- Visualize customer segments
- Profile each customer cluster
- Generate marketing recommendations
- Save the trained model and scaler for future predictions

---

## 📂 Dataset

| Property | Details |
|----------|---------|
| **Dataset** | Mall Customers Dataset |
| **Records** | 200 Customers |
| **Features** | 5 |
| **Missing Values** | None |

### Dataset Features

| Feature | Description |
|----------|-------------|
| CustomerID | Unique customer identifier (removed before training) |
| Gender | Customer gender (label encoded during preprocessing) |
| Age | Customer age |
| Annual Income (k$) | Annual income in thousand dollars |
| Spending Score (1-100) | Spending behavior score assigned by the mall |

---

## ⚙️ Technologies Used

| Technology | Purpose |
|------------|---------|
| Python | Programming Language |
| Pandas | Data manipulation |
| NumPy | Numerical computations |
| Matplotlib | Data visualization |
| Seaborn | Statistical visualization |
| Scikit-learn | Machine Learning |
| Joblib | Model persistence |

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

### 🟢 High Income High Spenders
- VIP memberships
- Premium product recommendations
- Exclusive rewards and loyalty programs

### 🔵 High Income Low Spenders
- Personalized promotions
- Product bundles
- Loyalty incentives to increase purchases

### 🟠 Young High Spenders
- Trend-focused products
- Student discounts
- Social media marketing campaigns

### 🟣 Young Average Spenders
- Personalized recommendations
- Seasonal promotions
- Customer engagement campaigns

### 🟡 Older Average Spenders
- Repeat purchase incentives
- Personalized services
- Family-oriented promotions

### 🔴 Low Income Low Spenders
- Budget-friendly products
- Discount offers
- Coupon campaigns

---

## 📁 Project Structure

```text
Customer-Segmentation-KMeans/
│
├── Analysis_Model.ipynb
├── Mall_Customers.csv
├── Mall_Customers_Clustered.csv
├── customer_segmentation.csv
├── KMeans_Model.pkl
├── StandardScaler.pkl
├── README.md
```

---


## 👤 Author

**Amalki Fernando**
