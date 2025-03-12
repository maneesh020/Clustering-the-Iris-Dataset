# Clustering the Iris Dataset

## Overview
This project applies **clustering techniques** to the well-known **Iris dataset** to identify natural groupings in the data. The two clustering algorithms implemented are:
- **KMeans Clustering**
- **Hierarchical Clustering**

## Dataset
The **Iris dataset** consists of **150 samples** from three different species of iris flowers:
- Setosa
- Versicolor
- Virginica

Each sample has **four features**:
- Sepal length
- Sepal width
- Petal length
- Petal width

Since this is an **unsupervised learning problem**, the species column is ignored, and clustering is performed only on the feature set.

## Project Structure
```
|-- iris-clustering/
    |-- iris_clustering.ipynb  # Jupyter Notebook with full implementation
    |-- README.md              # Project documentation
```

## Clustering Algorithms
### 1. KMeans Clustering
**Description:** KMeans is a centroid-based clustering algorithm that partitions data into `K` clusters. The algorithm works by:
- Randomly selecting `K` cluster centroids
- Assigning each data point to the nearest centroid
- Updating centroids based on cluster assignments
- Repeating the process until convergence

**Why KMeans is suitable for the Iris dataset?**
- The dataset has well-separated clusters, making KMeans an effective choice.
- It efficiently groups similar flowers based on numerical feature similarity.

**Implementation Steps:**
- Standardize the dataset using `StandardScaler`.
- Apply `KMeans` clustering with `n_clusters=3`.
- Visualize the clusters using scatter plots.

### 2. Hierarchical Clustering
**Description:** Hierarchical Clustering builds a tree-like hierarchy of clusters using a **bottom-up (agglomerative)** or **top-down (divisive)** approach.

**Why Hierarchical Clustering is suitable for the Iris dataset?**
- It provides a **dendrogram**, which gives insights into cluster relationships.
- No need to predefine the number of clusters.

**Implementation Steps:**
- Standardize the dataset using `StandardScaler`.
- Apply **Agglomerative Clustering** with `n_clusters=3`.
- Visualize clusters using scatter plots and a dendrogram.

## Results and Observations
- **KMeans Clustering** successfully grouped the dataset into three clusters.
- **Hierarchical Clustering** provided an informative **dendrogram** that confirmed natural divisions in the data.
- Both algorithms produced similar results, indicating strong natural clustering within the dataset.


## Author
- **Name:** Maneeshkumar G
- **Contact:** maneeshkumar1924@gmail.com

