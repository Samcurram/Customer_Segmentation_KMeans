# Customer_Segmentation_KMeans
A K-Means Clustering project to group mall customers based on their annual income and spending score. Implemented using Python, Scikit-learn, and the Elbow Method to identify target customer segments for marketing strategies.
# PRODIGY_DS_03: Customer Segmentation using K-Means Clustering

## 📄 Project Overview
This project implements **K-Means Clustering** to analyze a dataset of mall customers. The goal is to group customers based on their **Annual Income** and **Spending Score** to uncover meaningful patterns that can assist in marketing strategies.

This task is part of the **Prodigy InfoTech Data Science Internship** curriculum.

## 📊 Dataset
- **Source:** [Mall Customer Segmentation Data (Kaggle)](https://www.kaggle.com/vjchoudhary7/customer-segmentation-tutorial-in-python)
- **Description:** The dataset contains information about customers including:
  - CustomerID
  - Gender
  - Age
  - Annual Income (k$)
  - Spending Score (1-100)

## 🛠️ Technologies Used
- **Python** (Programming Language)
- **Google Colab** (Development Environment)
- **Pandas** (Data Manipulation)
- **Matplotlib & Seaborn** (Data Visualization)
- **Scikit-learn** (Machine Learning / K-Means)
- **KaggleHub** (Dataset Loading)

## 🔍 Methodology
1. **Data Loading:** Fetched the dataset dynamically using `kagglehub`.
2. **Data Preprocessing:** Selected relevant features (`Annual Income` and `Spending Score`) for clustering.
3. **Elbow Method:** Used the Within-Cluster Sum of Square (WCSS) to determine the optimal number of clusters ($K=5$).
4. **Model Training:** Trained the K-Means model with 5 clusters.
5. **Visualization:** Plotted the clusters and centroids to interpret the customer segments.

## 📈 Results / Cluster Interpretation
The analysis identified **5 distinct customer segments**:
1.  **Cluster 1 (Green):** High Income, High Spending -> *Target Group (VIPs)*
2.  **Cluster 2 (Red):** High Income, Low Spending -> *Careful Spenders*
3.  **Cluster 3 (Cyan):** Low Income, High Spending -> *Careless Spenders*
4.  **Cluster 4 (Magenta):** Low Income, Low Spending -> *Sensible Spenders*
5.  **Cluster 5 (Blue):** Average Income, Average Spending -> *Standard Customers*

## 🚀 How to Run
1. Open the file `PRODIGY_DS_03.ipynb` in Google Colab or Jupyter Notebook.
2. Ensure you have the required libraries installed:
   ```bash
   pip install kagglehub pandas matplotlib seaborn scikit-learn
