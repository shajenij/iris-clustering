# Iris Dataset Clustering

## Project Overview

This project applies unsupervised machine-learning techniques to the Iris
dataset. The objective is to discover natural groups of flowers using their
numerical measurements without providing the known species labels to the
clustering algorithms.

## Dataset

The Iris dataset is loaded from the scikit-learn library.

It contains 150 flower observations and four numerical features:

- Sepal length
- Sepal width
- Petal length
- Petal width

The species column is removed before clustering because it contains the known
class labels.

## Preprocessing

The following preprocessing steps were performed:

1. Loaded the Iris dataset from scikit-learn.
2. Converted the data into a pandas DataFrame.
3. Inspected its shape, data types, missing values and duplicate rows.
4. Removed the species column.
5. Standardized the four numerical features using StandardScaler.

## Clustering Algorithms

### KMeans Clustering

KMeans divides the observations into groups around cluster centroids. The
Elbow Method was used to support the selection of three clusters.

### Hierarchical Clustering

Agglomerative hierarchical clustering begins with individual observations and
gradually merges similar clusters. Ward linkage was used, and a dendrogram was
created to display the cluster hierarchy.

## Visualizations

The notebook contains:

- Elbow Method graph
- KMeans cluster scatter plot
- Hierarchical clustering dendrogram
- Hierarchical cluster scatter plot

## Technologies Used

- Python
- Google Colab
- pandas
- NumPy
- scikit-learn
- SciPy
- Matplotlib
- Seaborn

## Repository Contents

- `Iris_Clustering_Assignment.ipynb` — complete clustering notebook
- `README.md` — project documentation

## Conclusion

Both KMeans and hierarchical clustering discovered meaningful structure in
the Iris measurements. Flowers with short and narrow petals formed a clearly
separated group, while the remaining groups showed some overlap.
