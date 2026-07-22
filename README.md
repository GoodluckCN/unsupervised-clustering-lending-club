# Unsupervised Machine Learning: Clustering Analysis

[![Python](https://img.shields.io/badge/Python-3.8%2B-blue.svg)](https://www.python.org/)
[![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-Clustering-orange.svg)](https://scikit-learn.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

## 📌 Project Overview
This repository contains a comprehensive exploration of **unsupervised machine learning clustering techniques**, specifically focusing on **K-Means Clustering** and **Hierarchical (Agglomerative) Clustering**. The project starts with a foundational 2D coordinate example to visualize cluster boundaries and dendrograms, and extends to a practical financial application utilizing a subset of the **Lending Club** dataset to segment loan applications based on financial health, loan parameters, and purpose.

---
# 📊 Key Datasets & Features
- Simple Clustering Data (Simple_clustering_data_example.csv): A toy 2D coordinate dataset used to demonstrate algorithmic behavior, centroid optimization, and dendrogram construction.
- Lending Club Dataset Subset (LendingClub_small.csv): Financial records containing numerical and categorical attributes:
-- Loan Attributes: loan_amnt, int_rate, loan_status
-- Borrower Demographics: annual_inc, emp_length, pub_rec, home_ownership (One-hot encoded)
-- Loan Purpose: One-hot encoded categories (e.g., debt consolidation, credit card, medical, etc.)

# 🛠️ Methodology & Implementation
- Data Preprocessing: Handled categorical variables using One-Hot Encoding for loan purposes and applied StandardScaler to normalize features with varying scales and units.
- K-Means Clustering:
-- Initialized cluster centers and optimized partitions iteratively.
-- Visualized spatial distributions and cluster assignments using matplotlib and seaborn.
- Hierarchical Agglomerative Clustering:
-- Built linkage matrices using Ward's method and Euclidean distance metrics.
-- Generated and truncated dendrograms to analyze hierarchical tree structures and determine optimal cluster cutoff thresholds.

# 🚀 Getting Started
Prerequisites
Make sure you have Python 3.8+ installed. Clone this repository and install the dependencies: 
Bash 
git clone [https://github.com/your-username/unsupervised-clustering-lending-club.git](https://github.com/your-username/unsupervised-clustering-lending-club.git)
cd unsupervised-clustering-lending-club
pip install -r requirements.txt

Running the Analysis
Launch Jupyter Notebook to explore the step-by-step implementation: jupyter notebook

# 📈 Results & Visualizations
Dendrogram Analysis: Identifies natural hierarchical breaks in data groupings.
K-Means Partitioning: Successfully segments borrowers into distinct profiles based on income, interest rates, and loan amounts.

# 📝 License
This project is licensed under the MIT License - see the LICENSE file for details.


## 📂 Repository Structure
```text
├── data/                               # Dataset files
│   ├── Simple_clustering_data_example.csv
│   └── LendingClub_small.csv
├── notebooks/                          # Jupyter Notebooks containing the lab analysis
│   └── clustering_lab.ipynb
├── outputs/                            # Generated plots and visualizations
│   ├── dendrogram.png
│   └── kmeans_clusters.png
├── requirements.txt                    # Python dependencies
└── README.md                           # Project documentation
