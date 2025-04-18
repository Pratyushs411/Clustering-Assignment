# Breast Cancer Clustering Analysis

This project performs a clustering-based exploratory analysis on the **Breast Cancer Wisconsin (Diagnostic)** dataset using various clustering algorithms and preprocessing techniques.

## 📁 Dataset

- **Source**: [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/Breast+Cancer+Wisconsin+(Diagnostic))
- **Files Used**: `wdbc.data`, `wdbc.names`
- **Attributes**: 30 real-valued features from digitized images of breast masses

## 🧪 Objective

To evaluate the impact of different preprocessing techniques on clustering quality using:

### Clustering Algorithms
- K-Means
- Agglomerative (Hierarchical)
- Mean Shift

### Preprocessing Techniques
- None
- Normalization
- Transformation (PowerTransformer)
- PCA
- T+N (Transformation + Normalization)
- T+N+PCA

### Evaluation Metrics
- Silhouette Score
- Calinski-Harabasz Index
- Davies-Bouldin Index

## 🛠 How to Use

1. Upload `wdbc.data` and `wdbc.names` to your Colab/Notebook environment.
2. Run the notebook.
3. Review printed tables and `wdbc_clustering_results.csv` for results.

## 📊 Output

An evaluation CSV and optional visualizations are generated comparing clustering performance across techniques and clusters (3–5).

## 🧾 Conclusion

- **PCA with KMeans** often yields compact clusters.
- **Mean Shift** automatically identifies clusters but is slower and can be inconsistent across preprocessing.
- Preprocessing (T+N+PCA) tends to stabilize results.
