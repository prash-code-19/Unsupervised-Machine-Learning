# Unsupervised Learning

This folder contains Jupyter notebooks exploring unsupervised machine-learning techniques, including clustering, dimensionality reduction, and anomaly detection. The examples use scikit-learn's built-in Iris dataset, generated sample data, and an included thyroid dataset.

## Contents

| Notebook or file | Topics |
| --- | --- |
| [`k_means_clustering.ipynb`](./k_means_clustering.ipynb) | K-means clustering and selecting the number of clusters |
| [`k_means_iris.ipynb`](./k_means_iris.ipynb) | K-means applied to the Iris dataset |
| [`hierarchical.ipynb`](./hierarchical.ipynb) | Hierarchical clustering, dendrograms, and agglomerative clustering |
| [`dbscan.ipynb`](./dbscan.ipynb) | Density-based clustering, including non-linear sample data |
| [`PCA.ipynb`](./PCA.ipynb) | Principal Component Analysis (PCA) for dimensionality reduction |
| [`anomaly_detection.ipynb`](./anomaly_detection.ipynb) | Anomaly detection with Isolation Forest and Local Outlier Factor |
| [`thyroid_dataset.csv`](./thyroid_dataset.csv) | Local dataset used by the anomaly-detection notebook |

## Getting started

### Requirements

- Python 3.9 or later
- Jupyter Notebook or JupyterLab

### Setup

From this folder, create and activate a virtual environment, then install the notebook dependencies:

```bash
python -m venv .venv
```

On Windows:

```powershell
.\.venv\Scripts\Activate.ps1
```

On macOS or Linux:

```bash
source .venv/bin/activate
```

Install the packages used by the notebooks and start Jupyter:

```bash
python -m pip install --upgrade pip
python -m pip install jupyter numpy pandas matplotlib seaborn scikit-learn scipy kneed
jupyter lab
```

Open a notebook in Jupyter and run its cells from top to bottom. The anomaly-detection notebook reads `thyroid_dataset.csv` by a relative path, so launch Jupyter from this folder or update the path if you run it elsewhere. The other examples use scikit-learn's built-in datasets or generated data.

## Suggested learning path

Start with K-means to learn centroid-based clustering, then compare it with hierarchical clustering and DBSCAN. Explore PCA as a dimensionality-reduction technique, and finish with the anomaly-detection examples.

## Notes

- Notebooks are intended to be run independently; restart the kernel and run all cells if variables are missing.
- `.gitignore` excludes generated Python and Jupyter files, local environments, and local editor settings. The CSV dataset is intentionally kept under version control.
