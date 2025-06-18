# Iris-Dataset-Clustering-Analysis

# Project Overview
This project applies K-Means and DBSCAN clustering algorithms on the Iris dataset to analyze and compare clustering performance. Evaluation is done using silhouette scores, and results are visualized using Principal Component Analysis (PCA) for dimensionality reduction.

# Dataset Information
Name: Iris.csv

# Features:

Sepal Length

Sepal Width

Petal Length

Petal Width

# Objective: 
Cluster the data points into meaningful groups without predefined labels.

# Tech Stack
Programming Language: Python

Libraries Used:

pandas, numpy — Data handling

matplotlib, seaborn — Visualization

sklearn.cluster — K-Means & DBSCAN

sklearn.preprocessing — Standardization

sklearn.metrics — Silhouette score calculation

sklearn.decomposition — PCA

# Clustering Methods
1. K-Means Clustering
Uses 3 clusters (aligning with Iris species).

Calculates silhouette score for performance evaluation.

Visualized using PCA projection.

2. DBSCAN Clustering
Uses density-based clustering with eps=0.7, min_samples=5.

Identifies noise points (-1 labels) and filters them for silhouette analysis.

Often finds more distinct clusters than K-Means.

# Evaluation Metrics
Silhouette Score

K-Means: 0.4799

DBSCAN: 0.6018 (excluding noise points)

Higher score implies better-defined clusters.

# Visualization
Clusters are visualized using PCA-reduced 2D projections:

K-Means clusters shown using viridis color mapping.

DBSCAN clusters (including noise points) shown using coolwarm color mapping.

# Key Findings
K-Means forms moderately defined clusters, but some overlap exists.

DBSCAN provides better-separated clusters but identifies noise points.

The silhouette score indicates DBSCAN produces stronger cluster cohesion compared to K-Means.
