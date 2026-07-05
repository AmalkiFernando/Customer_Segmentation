# 🛍️ Customer Segmentation using K-Means Clustering

![Python](https://img.shields.io/badge/Python-3.10+-blue?logo=python&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-1.x-orange?logo=scikitlearn&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-2.x-150458?logo=pandas&logoColor=white)
![Status](https://img.shields.io/badge/Status-Complete-brightgreen)

A Machine Learning project that applies **K-Means Clustering** to segment mall customers into meaningful groups based on their purchasing behavior. The project combines **data preprocessing**, **feature scaling**, **cluster evaluation**, **visualization**, and **customer profiling** to generate actionable marketing insights.

---

# 📌 Project Overview

Customer segmentation helps businesses understand different groups of customers based on similar characteristics and purchasing patterns. By identifying these customer groups, businesses can design personalized marketing campaigns, improve customer engagement, and optimize sales strategies.

This project uses the **Mall Customers Dataset** and the **K-Means Clustering** algorithm to discover hidden customer segments using:

- Age
- Annual Income
- Spending Score

The optimal number of clusters was selected using both the **Elbow Method** and the **Silhouette Score**, followed by cluster profiling and marketing recommendations.

---

# 🎯 Project Objectives

- Perform Exploratory Data Analysis (EDA)
- Clean and preprocess customer data
- Encode categorical features
- Scale numerical features using StandardScaler
- Determine the optimal number of clusters
- Train a K-Means clustering model
- Evaluate clusters using Elbow Method and Silhouette Score
- Visualize customer segments
- Profile customer groups
- Generate marketing recommendations
- Save the trained model and scaler for future predictions

---

# 📂 Dataset Information

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

# ⚙️ Technologies Used

| Technology | Purpose |
|------------|---------|
| Python | Programming Language |
| Pandas | Data manipulation |
| NumPy | Numerical computation |
| Matplotlib | Data visualization |
| Seaborn | Statistical visualization |
| Scikit-learn | Machine Learning |
| Joblib | Save & Load trained models |
| Jupyter Notebook | Development Environment |

---

# 🔑 Key Techniques

- Exploratory Data Analysis (EDA)
- Label Encoding
- Feature Selection
- Feature Scaling (StandardScaler)
- K-Means Clustering
- Elbow Method
- Silhouette Score
- Cluster Profiling
- Data Visualization
- Model Persistence using Joblib

---

# 🤖 Machine Learning Pipeline

```text
Load Dataset
      │
      ▼
Exploratory Data Analysis (EDA)
      │
      ▼
Data Cleaning
      │
      ▼
Label Encoding
      │
      ▼
Feature Selection
      │
      ▼
Feature Scaling (StandardScaler)
      │
      ▼
Elbow Method
      │
      ▼
Silhouette Score
      │
      ▼
Optimal K Selection
      │
      ▼
Train K-Means Model
      │
      ▼
Assign Cluster Labels
      │
      ▼
Cluster Profiling
      │
      ▼
Customer Visualization
      │
      ▼
Marketing Recommendations
      │
      ▼
Save Model & Outputs
```

---

# 📈 Choosing the Optimal Number of Clusters

The optimal number of clusters was evaluated using both the **Elbow Method** and **Silhouette Score**.

| K | Inertia (WCSS) | Silhouette Score |
|---|---------------:|-----------------:|
| 2 | Replace | Replace |
| 3 | Replace | Replace |
| 4 | Replace | Replace |
| 5 | Replace | Replace |
| **6** | **Replace** | **Replace** ✅ |
| 7 | Replace | Replace |
| 8 | Replace | Replace |
| 9 | Replace | Replace |
| 10 | Replace | Replace |

> **Final Model:** K = **6** clusters were selected based on the Elbow Method and Silhouette Score.

---

# 📊 Cluster Summary

| Cluster | Segment | Customer Count | Average Age | Average Income | Average Spending |
|---------|----------------------------|---------------:|------------:|---------------:|-----------------:|
| 0 | Older Average Spenders | 45 | 56.33 | 54.27 | 49.07 |
| 1 | Young Average Spenders | 39 | 26.79 | 57.10 | 48.13 |
| 2 | High Income Low Spenders | 33 | 41.94 | 88.94 | 16.97 |
| 3 | High Income High Spenders | 39 | 32.69 | 86.54 | 82.13 |
| 4 | Young High Spenders | 23 | 25.00 | 25.26 | 77.61 |
| 5 | Low Income Low Spenders | 21 | 45.52 | 26.29 | 19.38 |

---

# 💡 Marketing Recommendations

### 🟢 High Income High Spenders
- VIP membership programs
- Premium product recommendations
- Exclusive rewards and loyalty programs

### 🔵 High Income Low Spenders
- Personalized promotions
- Product bundles
- Loyalty incentives to increase purchases

### 🟠 Young High Spenders
- Trend-focused products
- Student discounts
- Social media campaigns

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
- Discount campaigns
- Coupon offers

---

# 📊 Visualizations Included

The notebook includes the following visualizations:

- Age Distribution
- Annual Income Distribution
- Spending Score Distribution
- Gender Distribution
- Elbow Method
- Silhouette Score
- Customer Segmentation Scatter Plot
- Age vs Spending Score
- Cluster-wise Boxplots
- Customer Count by Segment

---

# 💾 Project Outputs

| File | Description |
|------|-------------|
| Analysis_Model.ipynb | Complete Machine Learning notebook |
| Mall_Customers.csv | Original dataset |
| Mall_Customers_Clustered.csv | Dataset with cluster labels |
| KMeans_Model.pkl | Saved K-Means model |
| StandardScaler.pkl | Saved StandardScaler |
| README.md | Project documentation |

---

# 📁 Repository Structure

```text
Customer-Segmentation-KMeans/
│
├── Analysis_Model.ipynb
├── Mall_Customers.csv
├── Mall_Customers_Clustered.csv
├── KMeans_Model.pkl
├── StandardScaler.pkl
├── requirements.txt
└── README.md
```

---

# 🚀 Installation

Clone the repository:

```bash
git clone https://github.com/your-username/Customer-Segmentation-KMeans.git
cd Customer-Segmentation-KMeans
```

Install the required libraries:

```bash
pip install -r requirements.txt
```

Launch Jupyter Notebook:

```bash
jupyter notebook
```

---

# 🔮 Predicting New Customers

The trained model and scaler are saved using **Joblib**, allowing new customer data to be classified without retraining the model.

Workflow:

1. Load the saved StandardScaler
2. Scale the new customer data
3. Load the saved K-Means model
4. Predict the customer cluster
5. Identify the customer segment

---

# 📌 Future Improvements

- Experiment with additional customer features
- Compare K-Means with DBSCAN and Hierarchical Clustering
- Deploy the model as a web application using Streamlit
- Build an interactive customer segmentation dashboard
- Automate customer profile generation

---

# 📖 Conclusion

This project successfully demonstrates how **K-Means Clustering** can be applied to identify meaningful customer segments using **Age**, **Annual Income**, and **Spending Score**. The resulting clusters provide valuable business insights that support personalized marketing strategies and data-driven decision-making.

The trained model, scaler, and clustered dataset are saved, allowing new customer data to be segmented without retraining the model.

---

# 👩‍💻 Author

**Amalki Fernando**

🎓 Bachelor of Information Technology (BIT)
