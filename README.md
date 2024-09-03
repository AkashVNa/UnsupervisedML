Aim:
  Perform machine learning by python on an unlabelled data.

Dataset:
  Use the Iris dataset available in the sklearn library.

Data Preprocessing:
  The dataset consists of 150 rows and 4 columns.
  No null values, duplicate rows are present in the dataset.
  Checking for outliers:
    mean and median seem to show no huge variation except maybe petal length (cm).
    all the features are showing acceptable levels of skewness.
    Thus there is no need to remove outliers.
  Data is scaled using Standard Scaler to facilitate better machine learning.

Data Processing:
  Since data is unlabelled, unsupervised machine learning methods are applicable. 
  Kmeans clustering and Agglomerative clustering methods are used for this purpose.
  Choosing the number of clusters:
    KMeans Clustering: Elbow method is used to determine the n_cluster parameter in this method.
    Agglomerative Clustering: Dendrogram is used to determine the n_cluster parameter in this method.

Visual Representations used:
  1. Plot to determine the n_clusters elbow method in KMeans clustering.
  2. Scatterplots to view the distribution of different features through Kmeans predicted clusters.
  3. Dendrogram plot to determine the n_clusters in Agglomerative CLustering.
  4. Scatterplots to view the distribution of different features through Agglomerative predicted clusters.


Inferences:
  The agglomerate heirarchichal clustering seems to fare better than kmeans clustering even though there scores are very similar(approximately 0.447 vs 0.444). 
  The data is of very small size so the developed models might not be of great reliability. 
  The number of clusters are found to be 3 in both cases so three clusters are produced.
