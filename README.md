# Unsupervised-ML

Beginner-friendly unsupervised machine learning notebooks in Python. Right now the repo covers **K-Means clustering**: how it works, how to choose the number of clusters (K), and how to apply it to a real dataset.

## Notebooks

| Notebook | Dataset | What it covers |
|----------|---------|----------------|
| `Kmeans.ipynb` | Synthetic data (`make_blobs`, 1000 points, 4 centers) | K-Means basics, Elbow method, automatic elbow detection with `kneed`, Silhouette score |
| `KmeansforIris.ipynb` | Iris dataset (`load_iris`) | Feature scaling, PCA (4D → 2D), Elbow method, K-Means with K = 3, cluster centers plot |

## Topics Covered

- K-Means clustering with scikit-learn
- Choosing K using the **Elbow method** (WCSS / inertia)
- Finding the elbow automatically with **KneeLocator** (`kneed`)
- Choosing K using the **Silhouette score**
- Feature scaling with `StandardScaler`
- Dimensionality reduction with **PCA** for visualization
- Visualizing clusters and centroids with seaborn

## Tech Stack

Python, scikit-learn, seaborn, pandas, kneed, Jupyter Notebook

## How to Run

```bash
git clone https://github.com/junaid0994/Unsupervised-ML.git
cd Unsupervised-ML
pip install scikit-learn seaborn pandas kneed jupyter
jupyter notebook
```

Then open any `.ipynb` file and run the cells in order.

## Planned

More unsupervised algorithms will be added as I learn them (for example Hierarchical Clustering and DBSCAN).

## Author

**Junaid Ashraf**
[GitHub](https://github.com/junaid0994) | [LinkedIn](https://www.linkedin.com/in/junaid-ashraf-53123b37a/)
