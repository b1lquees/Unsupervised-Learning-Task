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
| `Concepts.ipynb` | Foundational theory of unsupervised learning — clustering vs. dimensionality reduction, distance metrics, and small toy-data demos | Synthetic/toy data (generated in-notebook) |
| `ClusteringHAR.ipynb` | Full clustering case study: preprocessing, K-Means, Hierarchical/Agglomerative clustering, DBSCAN, Gaussian Mixture Models, Mean Shift, algorithm comparison, and model interpretation (feature importance, permutation importance, SHAP, PDP) | `data/train.csv` (HAR) |
| `DRDigits.ipynb` | Dimensionality reduction case study on handwritten digit images (PCA, and related techniques) | `sklearn.datasets.load_digits` (built-in, no file needed) |

`ClusteringHAR.ipynb` reads the dataset with a relative path, so it must be
run from within the `notebooks/` folder (as it is laid out in this repo):

```python
har = pd.read_csv('../data/train.csv')
```

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
