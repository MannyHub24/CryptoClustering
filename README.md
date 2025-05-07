
# Module 19 Challenge: Cryptocurrency Clustering

## Overview

In this challenge, we used unsupervised machine learning techniques to analyze and cluster cryptocurrencies based on their price change behaviors over 24 hours and 7 days. The goal was to identify natural groupings in the data and understand how dimensionality reduction affects clustering results.

## Steps Completed

1. **Data Preparation**
   - Loaded `crypto_market_data.csv` into a Pandas DataFrame.
   - Explored the data and checked for missing values.
   - Scaled the numerical features using `StandardScaler`.

2. **Elbow Method for K-Means**
   - Used the elbow method to determine the optimal number of clusters (`k`) on the scaled data.
   - Found that `k=4` was the best choice.

3. **K-Means Clustering on Scaled Data**
   - Applied K-Means with `k=4` and visualized the clusters using `hvplot`.

4. **Principal Component Analysis (PCA)**
   - Reduced the scaled data to 3 principal components.
   - Retained ~88.5% of the variance.
   - Re-ran the elbow method and confirmed `k=4` was still optimal.

5. **K-Means Clustering on PCA Data**
   - Re-clustered the PCA-reduced data.
   - Visualized the results using both 2D and 3D plots.

6. **Comparison**
   - Compared cluster results between original and PCA-reduced data using side-by-side plots.
   - Noted that PCA made clusters more compact and easier to visualize.

## Final Thoughts

Using PCA helped simplify the data while preserving most of its structure. Clusters became more defined, and visualizations were easier to interpret, all while maintaining consistent clustering performance.

---

### Tools Used

- Python
- Pandas
- Scikit-learn
- hvPlot
- Plotly
- Matplotlib

## Author 

Manuel Guevara

