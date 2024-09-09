# Crypto Clustering

## Overview
This project involves clustering cryptocurrency data to identify different groups or clusters of cryptocurrencies based on their price change patterns over time. The analysis is conducted using the K-Means clustering algorithm and involves both feature scaling and dimensionality reduction techniques like Principal Component Analysis (PCA) to optimize the clustering process.

## Libraries/Language
- Python 3.12
- Jupyter Notebook
- Pandas
- Numpy
- Scikit-learn
- Matplotlib

## Project Summary
The notebook follows these steps:

1. **Data Loading**: Loads the cryptocurrency data, which includes features such as price changes over different periods.
2. **Data Preprocessing**: Scales the data to standardize the range of features.
4. **K-Means Clustering**: Applys the K-Means algorithm to both the original scaled data and the PCA-transformed data to get Inertia, Silhouette, Calinski Harabasz scores.
5. **Elbow Curves**: Plots Elbow Curves for both the scaled data and the PCA-reduced data to determine the optimal number of clusters for K-Means.
6. **Principal Component Analysis (PCA)**: Reduces the features to three principal components to simplify the clustering process while retaining most of the variance.
7. **Visualization**: Visualizes the clustering results using scatter plots to compare the original features and PCA-reduced features.

## Results
**Elbow Curve Analysis*: Indicates that the optimal number of clusters is 4, both for the original scaled dataset and the PCA-reduced scaled dataset.
**Cluster Visualizations*: Show that the clusters formed using PCA-transformed dataset closely match those formed using the original scaled data, confirming that the dimensionality reduction retained the critical variance in the data.
**Conclusion*: Using PCA for feature reduction does not significantly impact the clustering quality, making it a suitable choice for reducing computational complexity while preserving performance.

## Works Cited
* Chat GBT for plotting using hvplot and readMe template

## License
GNU GENERAL PUBLIC LICENSE.
