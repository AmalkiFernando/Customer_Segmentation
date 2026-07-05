# Customer Segmentation using K-Means Clustering

A machine learning project that segments mall customers into meaningful groups using the **K-Means Clustering** algorithm. The project applies data preprocessing, feature scaling, cluster analysis, visualization, and marketing recommendations to better understand customer behavior.

---

## Project Overview

Customer segmentation is a technique used to group customers with similar characteristics and purchasing behaviors. By identifying these groups, businesses can create targeted marketing strategies, improve customer satisfaction, and optimize business decisions.

This project uses the **Mall Customers Dataset** to perform unsupervised learning using **K-Means Clustering**.

---

## Dataset

**Dataset:** Mall Customers Dataset

### Features

- CustomerID
- Gender
- Age
- Annual Income (k$)
- Spending Score (1-100)

---

## Objectives

- Explore customer data
- Clean and preprocess the dataset
- Perform feature scaling
- Determine the optimal number of clusters
- Apply K-Means clustering
- Visualize customer segments
- Profile each customer segment
- Generate marketing recommendations
- Save the trained model and scaler

---

## Machine Learning Workflow

1. Import Libraries
2. Load Dataset
3. Exploratory Data Analysis (EDA)
4. Data Cleaning
5. Label Encoding
6. Feature Selection
7. Feature Scaling
8. Elbow Method
9. Silhouette Score
10. Train K-Means Model
11. Cluster Profiling
12. Data Visualization
13. Marketing Recommendations
14. Save Model & Outputs

---

## Key Techniques

- K-Means Clustering
- Feature Scaling (StandardScaler)
- Label Encoding
- Elbow Method
- Silhouette Score
- Cluster Profiling
- Data Visualization
- Model Persistence (Joblib)

---

## Technologies Used

- Python 3.10+
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Joblib
- Jupyter Notebook

---

## Visualizations

The project includes several visualizations:

- Customer Age Distribution
- Annual Income Distribution
- Spending Score Distribution
- Gender Distribution
- Elbow Method
- Silhouette Score
- Customer Segmentation Scatter Plot
- Boxplots for Feature Distribution
- Customer Count by Segment

---

## Customer Segments

The K-Means model identifies six customer groups:

| Segment | Description |
|----------|-------------|
| Older Average Spenders | Older customers with moderate income and spending |
| Young Average Spenders | Young customers with average purchasing behavior |
| High Income Low Spenders | High-income customers with low spending habits |
| High Income High Spenders | Premium/VIP customers with high purchasing power |
| Young High Spenders | Young customers with high spending despite lower income |
| Low Income Low Spenders | Budget-conscious customers with low spending |

---

## Marketing Recommendations

### High Income High Spenders
- VIP memberships
- Premium products
- Exclusive promotions

### High Income Low Spenders
- Personalized offers
- Loyalty rewards
- Product bundles

### Young High Spenders
- Trend-focused campaigns
- Social media advertising
- Student discounts

### Young Average Spenders
- Personalized recommendations
- Seasonal promotions
- Loyalty programs

### Older Average Spenders
- Repeat purchase incentives
- Personalized services
- Family-oriented promotions

### Low Income Low Spenders
- Budget-friendly products
- Coupons
- Discount campaigns

---

## Project Outputs

The project generates the following files:

| File | Description |
|------|-------------|
| Mall_Customers_Clustered.csv | Dataset with assigned customer segments |
| KMeans_Model.pkl | Trained K-Means model |
| StandardScaler.pkl | Saved StandardScaler |
| Analysis_Model.ipynb | Complete analysis notebook |

---

## Predicting New Customers

The saved model can classify new customers into one of the identified customer segments without retraining.

Example workflow:

1. Load StandardScaler
2. Scale new customer data
3. Load trained K-Means model
4. Predict customer cluster
5. Assign customer segment

---

## Repository Structure

```
Customer-Segmentation-KMeans/
│
├── Analysis_Model.ipynb
├── Mall_Customers.csv
├── Mall_Customers_Clustered.csv
├── KMeans_Model.pkl
├── StandardScaler.pkl
├── README.md
```

---

## Conclusion

This project successfully applies **K-Means Clustering** to segment customers based on age, annual income, and spending score. The identified customer groups provide actionable marketing insights that can help businesses improve customer engagement, personalize promotions, and support data-driven decision-making.
