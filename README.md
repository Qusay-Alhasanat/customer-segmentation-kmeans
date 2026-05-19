# 🛍️ Customer Segmentation using K-Means Clustering

## 📌 Project Overview
This project applies **K-Means Clustering**, an unsupervised machine learning algorithm, to segment customers based on their **annual income** and **spending behavior**.

The goal is to discover hidden patterns in customer data and group similar customers together to support better business decisions and marketing strategies.

---

## 🎯 Problem Statement
Businesses often struggle to understand different types of customers.  
The objective of this project is to:
- Identify distinct customer segments
- Understand spending behavior patterns
- Support targeted marketing strategies

---

## 📊 Dataset Description
The dataset contains customer information with the following features:

- Customer ID
- Gender
- Age
- Annual Income (k$)
- Spending Score (1–100)

After preprocessing, only relevant features were used:
- Annual Income
- Spending Score

---

## 🧹 Data Preprocessing
The following steps were applied:

- Renamed columns for consistency
- Handled missing values:
  - Numerical → Median
  - Categorical → Mode
- Removed irrelevant column (Customer ID)
- Standardized features using **StandardScaler**

---

## 📈 Exploratory Data Analysis (EDA)
Key insights:
- Majority of customers are between 30–40 years old
- Clear variation in spending behavior across income levels
- Negative correlation between income and spending score (-0.84)

---

## 🧠 Model Used
We used:

### K-Means Clustering
An unsupervised learning algorithm that groups data into clusters based on similarity.

### Why K-Means?
- Simple and efficient
- Works well with numeric data
- Ideal for customer segmentation

---

## 🔢 Optimal Number of Clusters
The **Elbow Method** was used to determine the optimal number of clusters.

Optimal K selected: **3**

---

## 📊 Results

The model identified 3 distinct customer segments:

### 🔴 Cluster 0: Careful Spenders
- Medium income
- Low spending

### 🟢 Cluster 1: Budget-Constrained Spenders
- Low income
- High spending

### 🔵 Cluster 2: High-Income Low Spenders
- High income
- Low spending

---

## 💡 Business Insights
- High-income customers are not always high spenders
- Low-income customers can still be high-value buyers
- Marketing strategies should be customized per segment

---

## 🛠️ Tools & Technologies
- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn

---

## 🚀 Key Takeaway
Customer segmentation helps businesses move from **general marketing** to **personalized targeting**, improving engagement and revenue.

---

## 📌 Future Improvements
- Try more clusters (K=4 or 5)
- Add demographic features (Age, Gender)
- Use advanced clustering methods (DBSCAN, Hierarchical Clustering)
