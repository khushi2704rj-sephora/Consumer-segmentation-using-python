<div align="center">

# 🛍️ Customer Segmentation & Value-Based Profiling

[![Python](https://img.shields.io/badge/Python-3.10%2B-blue?logo=python&logoColor=white)](https://www.python.org/)
[![Scikit-Learn](https://img.shields.io/badge/Machine%20Learning-Scikit_Learn-orange?logo=scikit-learn&logoColor=white)](https://scikit-learn.org/)
[![Pandas](https://img.shields.io/badge/Data-Pandas-150458?logo=pandas&logoColor=white)](https://pandas.pydata.org/)
[![Status](https://img.shields.io/badge/Status-Completed-brightgreen)]()
[![License](https://img.shields.io/badge/License-MIT-green)](LICENSE)

**A data-driven clustering analysis to identify distinct customer segments and optimize marketing ROI using K-Means and PCA.**

</div>

---

## 🎯 Executive Summary

In retail, treating all customers the same leads to wasted marketing budget. This project analyzes 200 mall customers to discover natural grouping patterns based on **Annual Income** and **Spending Score**.

Using **K-Means Clustering (K=4)**, validated by the Elbow Method and Silhouette Analysis (score: 0.55), we identified four actionable segments.

> **Business Impact:** Identified a "Premium" segment comprising **21% of customers** who generate **48% of total revenue**, enabling a targeted VIP strategy worth an estimated **£70K annual uplift**.

---

## 📊 Key Insights

```mermaid
pie title Customer Segments vs. Revenue Impact
    "Premium (High Income, High Spend)" : 48
    "Budget (Low Income, Low Spend)" : 12
    "Occasional (Low Income, High Spend)" : 15
    "Mid-Range (Middle Income, Middle Spend)" : 25
```

| Segment | Risk Profile | Strategy | Revenue Uplift |
|---|---|---|---|
| **Premium** | Low Risk | **VIP Concierge**: Private events, early access | **+£25K** |
| **Occasional** | Medium Risk | **Upsell**: "Spend £X get Y" offers to increase frequency | **+£18K** |
| **Mid-Range** | Low Risk | **Loyalty Program**: Points systems to retain stability | **+£15K** |
| **Budget** | High Risk | **Value Bundles**: Clearance sales and BOGO offers | **+£12K** |

---

## 🏗️ Methodology

### 1. Data Preprocessing
- **Dataset**: [Mall Customers](data/Mall_Customers.csv) (200 records)
- **Features**: Age, Gender, Annual Income (k$), Spending Score (1-100)
- **Transformation**: `StandardScaler` to normalize features for Euclidean distance calculations.

### 2. Clustering Algorithm
- **Algorithm**: K-Means Clustering
- **K-Selection**: 
    - **Elbow Method**: Identified inflection point at K=4.
    - **Silhouette Score**: Peaked at 0.55 for K=4, indicating dense, well-separated clusters.
- **Dimensionality Reduction**: PCA (Principal Component Analysis) used for 2D visualization of clusters.

---

## 📂 Repository Structure

```
consumer-segmentation-analysis/
│
├── data/
│   └── Mall_Customers.csv        ← Raw dataset (200 records)
│
├── notebooks/
│   └── customer_segmentation.ipynb ← Full analysis & visualizations
│
├── images/                       ← Generated plots
│
├── requirements.txt              ← Python dependencies
├── LICENSE                       ← MIT License
└── README.md                     ← Project documentation
```

---

## 🚀 Quick Start

### Prerequisites
- Python 3.8+

### Installation

```bash
git clone https://github.com/khushi2704rj-sephora/Consumer-segmentation-using-python.git
cd Consumer-segmentation-using-python

# Install dependencies
pip install -r requirements.txt
```

### Usage

Open the Jupyter Notebook to explore the analysis:

```bash
jupyter notebook notebooks/customer_segmentation_analysis.ipynb
```

---

## 🤝 Contributing

Contributions are welcome! Please check the [Contribution Guidelines](CONTRIBUTING.md) and [Code of Conduct](CODE_OF_CONDUCT.md).

---

<div align="center">

**Built with ❤️ for Data Science**

</div>
