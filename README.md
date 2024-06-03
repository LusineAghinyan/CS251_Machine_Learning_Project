# Colorectal Cancer Gene Expression Analysis

### Project Overview

This project focuses on analyzing gene expression data from colorectal cancer samples. By leveraging machine learning techniques, we want to find significant patterns and potential biomarkers that can contribute to better understanding and treatment of colorectal cancer.

### Goals

Data Exploration and Cleaning:

1. Understand how the data is structured and distributed.
2. Clean and preprocess the data to make it ready for analysis.

Dimensionality Reduction:

1. Reduce the complexity of gene expression data while maintaining crucial information.
2. Visualise the data to identify underlying patterns or clusters.

Machine Learning Modeling:

1. Build and evaluate models to classify cancer stages and identify important features.
2. Use clustering algorithms to investigate possible gene expression groups.

Insights and Interpretations:

1. Extract meaningful insights from the data analysis and modeling results.
2. Provide interpretations that can help us comprehend colorectal cancer biology.

### Table of Contents

1. Data Description
2. Data Preparation
3. Clustering Analysis
4. Comparison between Clustering Algorithms
5. Classical Algorithms
6. Comparison between Multi-class Classification Algorithms

### Data Description

Gene Expression Data:
This dataset includes gene expression levels from colorectal cancer samples.
- Data Structure: It consists of 1,935 rows and 64 columns.
- Columns: ID_REF provides gene IDs, indicating each row corresponds to a certain gene. Additional columns (e.g., GSM877126) likely represent microarray sample identifiers and gene expression levels.
- Purpose: Gene expression databases help analyze gene activity across different situations or therapies, aiding in determining gene regulation in cancer settings.

Patient Data:
This dataset focuses on clinical and demographic features of patients from whom samples were collected.
- Columns: ID_REF matches sample IDs in gene expression data, with additional features such as Age, Dukes classification, Gender, Location of cancer, Disease-free survival (DFS), DFS event, Adj_Radio, and Adj_Chem.

### Data Preparation

- Import necessary libraries.
- Dimensionality reduction techniques were employed.
- Data underwent clustering analysis using K-Means, Hierarchical Clustering, and DBSCAN.

### Clustering Analysis

- K-Means, Hierarchical Clustering, and DBSCAN were applied.
- Silhouette Scores were computed for each algorithm.
- Results indicated overlapping clusters and poor separation.

### Classical Algorithms

Several classical algorithms were tested for multi-class classification:

- Logistic Regression
- K-Nearest Neighbors
- Support Vector Machine
- Decision Tree
- Random Forest
- Gradient Boosting
- Stacking

### Insights

- Class Struggle: Classes with fewer samples were consistently difficult for most models, suggesting class imbalance.
- Model Selection: Logistic Regression and Gradient Boosting showed more consistency.
- Feature Engineering: Improved feature engineering and handling of imbalanced data might be necessary.