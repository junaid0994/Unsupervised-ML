# Unsupervised-ML

Beginner-friendly unsupervised machine learning notebooks in Python. Right now the repo covers **K-Means**, **Hierarchical Clustering**, **DBSCAN**, **PCA** and **Anomaly Detection** (DBSCAN, Isolation Forest, LOF): how each one works, how to choose its settings, and how to apply it to a dataset.

## Notebooks

| Notebook | Dataset | What it covers |
|----------|---------|----------------|
| `Kmeans.ipynb` | Synthetic data (`make_blobs`, 1000 points, 4 centers) | K-Means basics, Elbow method, automatic elbow detection with `kneed`, Silhouette score |
| `KmeansforIris.ipynb` | Iris dataset (`load_iris`) | Feature scaling, PCA (4D → 2D), Elbow method, K-Means with K = 3, cluster centers plot |
| `hierarchical_clustering.ipynb` | Iris dataset (`load_iris`) | Feature scaling, linkage matrix (Ward method), dendrogram, Agglomerative Clustering with 3 clusters |
| `DBSCAN.ipynb` | Iris dataset (`load_iris`) and `make_moons` (300 points, non-linear data) | Feature scaling, DBSCAN with `eps` and `min_samples`, noise points, K-Means vs DBSCAN on non-linear data |
| `DBSCAN_Anomalies.ipynb` | `make_moons` (500 points, noise = 0.1) | Feature scaling, DBSCAN with `eps = 0.18` and `min_samples = 5`, plotting the clusters, points labelled `-1` are the anomalies (noise) |
| `PCA.ipynb` | Iris dataset (`load_iris`) | Feature scaling, PCA with 2 components, explained variance ratio, principal components, 2D scatter plot coloured by species |
| `Isolation_Forest.ipynb` | Thyroid dataset (`thyroid_dataset.csv`, 6916 rows) | Feature scaling, **Isolation Forest** and **Local Outlier Factor (LOF)** with `contamination = 0.036`, counting outliers vs normal points, visualizing results with PCA (2D) |

## Topics Covered

- K-Means clustering with scikit-learn
- Choosing K using the **Elbow method** (WCSS / inertia)
- Finding the elbow automatically with **KneeLocator** (`kneed`)
- Choosing K using the **Silhouette score**
- **Hierarchical (Agglomerative) Clustering** with Ward linkage
- Reading a **dendrogram** to decide the number of clusters
- **DBSCAN** (density-based clustering) with `eps` and `min_samples`
- Why K-Means fails on non-linear (moon-shaped) data and DBSCAN works
- **Anomaly detection** with DBSCAN (points that belong to no cluster get label `-1`)
- **Anomaly detection** with **Isolation Forest** and **Local Outlier Factor (LOF)** on a real dataset
- The `contamination` setting (expected share of outliers)
- **PCA** (Principal Component Analysis): reducing features to 2D for plotting and checking how much variance each component keeps
- Feature scaling with `StandardScaler`
- Visualizing clusters, centroids and outliers with seaborn and matplotlib

## Tech Stack

Python, scikit-learn, scipy, seaborn, matplotlib, pandas, numpy, kneed, Jupyter Notebook

## How to Run

```bash
git clone https://github.com/junaid0994/Unsupervised-ML.git
cd Unsupervised-ML
pip install scikit-learn scipy seaborn matplotlib pandas numpy kneed jupyter
jupyter notebook
```

Then open any `.ipynb` file and run the cells in order.

`Isolation_Forest.ipynb` reads `thyroid_dataset.csv`, so keep that file in the same folder as the notebook.

## Planned

More unsupervised algorithms will be added as I learn them (for example Gaussian Mixture Models).

## Author

**Junaid Ashraf**
[GitHub](https://github.com/junaid0994) | [LinkedIn](https://www.linkedin.com/in/junaid-ashraf-53123b37a/)
