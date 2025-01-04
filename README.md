# Crime Data Clustering

This project performs clustering analysis on U.S. crime data using Hierarchical, K-Means, and DBSCAN algorithms. The aim is to identify the optimal number of clusters and derive meaningful inferences about crime patterns based on features like **Murder**, **Assault**, **Urban Population**, and **Rape**.

## Table of Contents
- [Data Description](#data-description)
- [Clustering Techniques](#clustering-techniques)
  - [Hierarchical Clustering](#hierarchical-clustering)
  - [K-Means Clustering](#k-means-clustering)
  - [DBSCAN Clustering](#dbscan-clustering)
- [Visualizations](#visualizations)
- [Inferences](#inferences)
- [Setup and Usage](#setup-and-usage)
- [Results](#results)

---

## Data Description
- **Murder**: Murder rates in different places of the United States.
- **Assault**: Assault rates in different places of the United States.
- **UrbanPop**: Urban population in different places of the United States.
- **Rape**: Rape rates in different places of the United States.

## Clustering Techniques
### Hierarchical Clustering
- Used **dendrograms** to identify the number of clusters.
- Applied **Agglomerative Clustering** to group similar regions.

### K-Means Clustering
- Used **Elbow Curve** to find the optimal number of clusters.
- Clustered data using K-Means and analyzed intra-cluster similarities.

### DBSCAN Clustering
- Applied **Density-Based Spatial Clustering** for identifying arbitrarily shaped clusters.
- Tuned `eps` and `min_samples` parameters for optimal clustering.

## Visualizations
- Dendrograms for hierarchical clustering.
- Elbow curve for K-Means optimization.
- Scatter plots for cluster visualization.

## Inferences
- Hierarchical and K-Means clustering identified consistent cluster patterns.
- DBSCAN was sensitive to parameter tuning but struggled with noise in the data (silhouette score: -0.268).
- Urban population and crime rates influence clustering significantly.

## Setup and Usage
1. Clone the repository:
   ```bash
   git clone https://github.com/R-Mahesh45/crime-data-clustering.git
   ```
2. Install required libraries:
   ```bash
   pip install pandas numpy matplotlib seaborn scipy scikit-learn
   ```
3. Run the clustering analysis:
   ```bash
   python clustering_analysis.py
   ```

## Results
- **Hierarchical Clustering**: X clusters were formed.
- **K-Means Clustering**: Y clusters were optimal based on the elbow method.
- **DBSCAN Clustering**: Challenging to form clusters due to noise.
