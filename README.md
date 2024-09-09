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

## Explanation of Analysis
The notebook follows these steps:

1. Data Loading: Load the cryptocurrency data, which includes features such as price changes over different periods.
2. Data Preprocessing: Scale the data to standardize the range of features.
3. Elbow Method for Optimal Clusters:
    * Perform the Elbow Method on both the scaled data and the PCA-reduced data to determine the optimal number of clusters for K-Means.
4. Principal Component Analysis (PCA): Reduce the feature space to two principal components to simplify the clustering process while retaining most of the variance.
5. K-Means Clustering:
    * Apply the K-Means algorithm to both the original scaled data and the PCA-transformed data.
6. Visualization: Visualize the clustering results using scatter plots to compare the original features and PCA-reduced features.

## Results
* Elbow Curve Analysis: Indicates that the optimal number of clusters is 4, both for the full feature set and the PCA-reduced set.
* Cluster Visualizations: Show that the clusters formed using PCA-transformed data closely match those formed using the original features, confirming that the dimensionality reduction retained the critical variance in the data.
* Conclusion: Using PCA for feature reduction does not significantly impact the clustering quality, making it a suitable choice for reducing computational complexity while preserving performance.

## Works Cited
* Chat GBT for plotting using hvplot and readMe template

## License
GNU GENERAL PUBLIC LICENSE.