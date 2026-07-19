# Unsupervised Machine Learning — Case Studies

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

### `data/`
Contains `train.csv`, the Human Activity Recognition (HAR) dataset: 561
smartphone accelerometer/gyroscope features across 7,352 samples, labeled
with 6 activity classes (`WALKING`, `WALKING_UPSTAIRS`, `WALKING_DOWNSTAIRS`,
`SITTING`, `STANDING`, `LAYING`). Used by `ClusteringHAR.ipynb`.

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
   git clone <your-repo-url>
   cd <repo-name>
   ```
2. Install dependencies:
   ```bash
   pip install numpy pandas matplotlib seaborn scikit-learn scipy shap
   ```
3. Launch Jupyter and open any notebook in `notebooks/`:
   ```bash
   jupyter notebook notebooks/
   ```
