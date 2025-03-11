# **Iris Dataset Analysis with PCA, t-SNE, and UMAP**

## **Overview**
This script loads the Iris dataset, processes it into an `AnnData` object, and applies dimensionality reduction techniques (PCA, t-SNE, and UMAP) to visualize the data. The results are plotted using `seaborn`.

## **Dependencies**
Ensure you have the following Python packages installed:

- `numpy`
- `pandas`
- `scanpy`
- `seaborn`
- `matplotlib`
- `scikit-learn`
- `anndata`

You can install them using:

```bash
pip install numpy pandas scanpy seaborn matplotlib scikit-learn anndata
```

## **Usage**
Run the script to:
1. Load the **Iris dataset**.
2. Convert it into an `AnnData` object.
3. Perform **PCA**, **t-SNE**, and **UMAP** for dimensionality reduction.
4. Visualize the embeddings with scatter plots colored by species.

## **Key Steps**
- **Load and preprocess** the dataset using `AnnData`.
- **Perform dimensionality reduction**:
  - PCA (`sc.pp.pca`)
  - t-SNE (`sc.tl.tsne`)
  - UMAP (`sc.pp.neighbors` and `sc.tl.umap`)
- **Visualize results** using `seaborn.scatterplot`.