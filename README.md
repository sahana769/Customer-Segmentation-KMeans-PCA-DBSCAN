# 🚀 Customer Segmentation using KMeans, PCA & DBSCAN

![Python](https://img.shields.io/badge/Python-3.10-blue?logo=python)
![Jupyter Notebook](https://img.shields.io/badge/Jupyter-Notebook-orange?logo=jupyter)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-0.24-green?logo=scikitlearn)

---

## 💡 Project Overview

This project performs **advanced customer segmentation** using **unsupervised machine learning techniques**.  
The goal is to group customers based on their purchasing behavior (Recency, Frequency, Monetary value) to enable targeted marketing, retention strategies, and revenue optimization.

**Techniques used:**
- **KMeans Clustering** → Main segmentation
- **PCA (Principal Component Analysis)** → Dimensionality reduction & visualization
- **DBSCAN** → Anomaly detection (outlier customers)

---

## 📝 Problem Statement

E-commerce businesses collect massive customer transaction data but often fail to extract actionable insights.  
This project aims to **segment customers** into meaningful groups based on their buying behavior, providing insights for:
- Targeted marketing campaigns  
- Personalized promotions  
- Customer retention strategies  
- Revenue optimization

---

## 📊 Dataset

- **Source:** [Online Retail Dataset (Kaggle)](https://www.kaggle.com/datasets/carrie1/ecommerce-data)  
- **Description:** Real transactions from a UK-based online retailer  
- **Key Features:**
  - `InvoiceNo` – Invoice number  
  - `StockCode` – Product code  
  - `Description` – Product name  
  - `Quantity` – Quantity purchased  
  - `InvoiceDate` – Transaction date  
  - `UnitPrice` – Price per unit  
  - `CustomerID` – Unique customer ID  
  - `Country` – Customer country  

> Used to calculate **RFM features** for clustering

---

## 🛠️ Libraries & Tools

- Python 3.x  
- pandas, numpy (data manipulation)  
- matplotlib, seaborn (visualization)  
- scikit-learn (StandardScaler, PCA, KMeans, DBSCAN, silhouette_score)  
- Jupyter Notebook  

---

## 🔄 Workflow

1. Import Libraries  
2. Load Dataset  
3. Data Cleaning (remove missing CustomerIDs, canceled transactions)  
4. Feature Engineering → Recency, Frequency, Monetary (RFM)  
5. Feature Scaling  
6. Dimensionality Reduction → PCA  
7. KMeans Clustering → Segment customers  
8. DBSCAN → Detect outliers / anomalies  
9. Cluster Visualization & Insights  
10. Business Insights & Conclusion  

---

## 📈 Key Insights

| Cluster | Characteristics | Recommended Strategy |
|---------|----------------|--------------------|
| 0       | High Recency, High Monetary, Frequent purchases | VIP customers → Loyalty programs, personalized promotions |
| 1       | Low Recency, Low Monetary, Infrequent purchases | Dormant customers → Re-engagement campaigns |
| 2       | Moderate values across RFM | Regular customers → Upsell products |
| -1      | Outliers (DBSCAN) | Investigate unusual behavior or potential fraud |

---

## 🖥️ How to Run

```bash
# Clone repository
git clone https://github.com/yourusername/Customer-Segmentation-KMeans-PCA-DBSCAN.git

# Install dependencies
pip install pandas numpy matplotlib seaborn scikit-learn jupyter

# Run notebook
jupyter notebook Customer-Segmentation.ipynb
