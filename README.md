# Unsupervised-ML

Beginner-friendly unsupervised machine learning notebooks in Python. Right now the repo covers **K-Means**, **Hierarchical Clustering** and **DBSCAN**: how each one works, how to choose its settings, and how to apply it to a real dataset.

## Notebooks

| Notebook | Dataset | What it covers |
|----------|---------|----------------|
| `Kmeans.ipynb` | Synthetic data (`make_blobs`, 1000 points, 4 centers) | K-Means basics, Elbow method, automatic elbow detection with `kneed`, Silhouette score |
| `KmeansforIris.ipynb` | Iris dataset (`load_iris`) | Feature scaling, PCA (4D → 2D), Elbow method, K-Means with K = 3, cluster centers plot |
| `hierarchial_clustering.ipynb` | Iris dataset (`load_iris`) | Feature scaling, linkage matrix (Ward method), dendrogram, Agglomerative Clustering with 3 clusters |
| `DBSCAN.ipynb` | Iris dataset (`load_iris`) and `make_moons` (300 points, non-linear data) | Feature scaling, DBSCAN with `eps` and `min_samples`, noise points, K-Means vs DBSCAN on non-linear data |

## Topics Covered

- K-Means clustering with scikit-learn
- Choosing K using the **Elbow method** (WCSS / inertia)
- Finding the elbow automatically with **KneeLocator** (`kneed`)
- Choosing K using the **Silhouette score**
- **Hierarchical (Agglomerative) Clustering** with Ward linkage
- Reading a **dendrogram** to decide the number of clusters
- **DBSCAN** (density-based clustering) with `eps` and `min_samples`
- Why K-Means fails on non-linear (moon-shaped) data and DBSCAN works
- Feature scaling with `StandardScaler`
- Dimensionality reduction with **PCA** for visualization
- Visualizing clusters and centroids with seaborn and matplotlib

## Tech Stack

Python, scikit-learn, scipy, seaborn, matplotlib, pandas, kneed, Jupyter Notebook

## How to Run

```bash
git clone https://github.com/junaid0994/Unsupervised-ML.git
cd Unsupervised-ML
pip install scikit-learn scipy seaborn matplotlib pandas kneed jupyter
jupyter notebook
```

Then open any `.ipynb` file and run the cells in order.

## Planned

More unsupervised algorithms will be added as I learn them (for example Gaussian Mixture Models and PCA in more depth).

## Author

**Junaid Ashraf**
[GitHub](https://github.com/junaid0994) | [LinkedIn](https://www.linkedin.com/in/junaid-ashraf-53123b37a/)
