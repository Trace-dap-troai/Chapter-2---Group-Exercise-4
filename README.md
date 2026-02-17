# Group Members

Munib Ahmed

Chech Trac, Way

Mehatab

## Objective

The objective of this exercise is to apply and compare two different clustering techniques on the same dataset used in Group Exercise 3.  
The goal is to understand the differences between partition-based clustering and density-based clustering methods.

---

## Dataset

This project uses the same dataset from Group Exercise 3.

Before applying clustering:

- Features were standardized using StandardScaler.
- PCA was applied to reduce the data to 2 dimensions for visualization purposes.

---

## Method 1: K-Means Clustering

K-Means is a partition-based clustering algorithm that divides data into k clusters by minimizing the distance between data points and their corresponding cluster centroids.

Chosen parameter:

- k = 2 clusters

Results:

- The dataset was divided into two clusters.
- Each data point was assigned to one of the two clusters.
- Clusters were visualized using PCA (2D projection).

Characteristics:

- Produces spherical clusters.
- Sensitive to initial centroid placement.
- Every data point is assigned to a cluster (no noise detection).

---

## Method 2: DBSCAN Clustering

DBSCAN (Density-Based Spatial Clustering of Applications with Noise) is a density-based clustering algorithm that groups data points based on density and can identify noise points.

Chosen parameters:

- eps = 0.5  
- min_samples = 5  

Results:

- The algorithm detected a certain number of clusters.
- Noise points were identified and labeled as -1.
- Clusters were visualized using PCA (2D projection).

Characteristics:

- Can detect arbitrarily shaped clusters.
- Identifies noise and outliers.
- Sensitive to parameter selection (eps and min_samples).

---

## Comparison: K-Means vs DBSCAN

Cluster Shape and Structure:

- K-Means creates compact, spherical clusters.
- DBSCAN can form clusters of arbitrary shape.

Sensitivity to Noise:

- K-Means assigns every point to a cluster and does not handle noise.
- DBSCAN can detect and label noise points.

Suitability for the Dataset:

- K-Means is suitable when clusters are well-separated and compact.
- DBSCAN is more suitable when the dataset contains noise or irregular cluster shapes.

---

## Conclusion

Both clustering methods were successfully applied to the dataset.

K-Means provided a clear partition into two clusters, while DBSCAN offered additional insight by detecting noise points and handling irregular cluster structures.

This exercise demonstrates the conceptual and practical differences between partition-based and density-based clustering techniques.
