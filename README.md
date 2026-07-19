# Unsupervised Machine Learning

A collection of notebooks covering the core concepts, algorithms, and practical
case studies for unsupervised machine learning: clustering, dimensionality
reduction, and model interpretation.

## Project Structure

```
.
├── data/
│   └── train.csv              # Human Activity Recognition (HAR) dataset
├── notebooks/
│   ├── Concepts.ipynb         # Core theory: distance metrics, clustering vs. DR
│   ├── ClusteringHAR.ipynb    # Clustering case study on the HAR dataset
│   └── DRDigits.ipynb         # Dimensionality reduction case study on Digits
└── README.md
```

### `notebooks/`

| Notebook | Topic | Dataset |
|---|---|---|
| `Concepts.ipynb` | Foundational theory of unsupervised learning — clustering vs. dimensionality reduction, distance metrics, and small toy-data demos | Synthetic data |
| `ClusteringHAR.ipynb` | Full clustering case study: preprocessing, K-Means, Hierarchical/Agglomerative clustering, DBSCAN, Gaussian Mixture Models, Mean Shift, algorithm comparison, and model interpretation (feature importance, permutation importance, SHAP, PDP) | `data/train.csv` (HAR) |
| `DRDigits.ipynb` | Dimensionality reduction case study on handwritten digit images (PCA, and related techniques) | `sklearn.datasets.load_digits`|

## Getting Started

1. Clone the repository:
   ```bash
   https://github.com/b1lquees/Unsupervised-Learning-Task.git
   cd Unsupervised-Learning-Task
   ```
2. Install dependencies:
   ```bash
   pip install numpy pandas matplotlib seaborn scikit-learn scipy shap
   ```

   ## Cluster Evaluation Metrics
- Silhouette Score
- Davies-Bouldin Index
- Calinski-Harabasz Index
- Inertia (Within-Cluster Sum of Squares)
- Adjusted Rand Index (ARI, vs true labels)

## Dimensionality Reduction Methods
- Principal Component Analysis (PCA)
- Kernel PCA
- t-SNE
- UMAP

## Model Interpretation
- Feature Importance
- Permutation Importance
- SHAP (SHapley Additive exPlanations)
- Partial Dependence Plots (PDP)

## Techniques Used
- Data Cleaning
- Data Preprocessing
- Feature Scaling (StandardScaler)
- Hyperparameter Tuning (Elbow Method, Silhouette Score, BIC, k-distance plot, bandwidth estimation)
- Model Comparison
- Cluster Visualization (before and after dimensionality reduction)
## Results
Five clustering algorithms and four dimensionality reduction methods were applied and evaluated. Their performances were compared using evaluation metrics and visualization graphs. Hyperparameters were tuned for every algorithm to improve performance.

**Best Clustering Algorithms:** K-Means and Gaussian Mixture Models

**Best Dimensionality Reduction Method:** UMAP 

## Author
Bilquees Ashfaq Jumani
