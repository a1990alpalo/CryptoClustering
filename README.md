# CryptoClustering

his project uses Python and unsupervised learning techniques to analyze and cluster cryptocurrencies based on their price changes over 24-hour and 7-day periods. By identifying patterns within the data, we aim to determine whether clustering can reveal insights into cryptocurrency price movements.

Project Overview
In this challenge, we leverage machine learning to determine if there are patterns in cryptocurrency price fluctuations. We'll use the K-means clustering algorithm on both raw data and Principal Component Analysis (PCA)-reduced data to identify clusters and compare the impact of dimensionality reduction on clustering outcomes.

Steps to Complete the Project
1. Setup and Preparation
Create a new repository named CryptoClustering and clone it to your local machine.
Load the dataset crypto_market_data.csv into a DataFrame and explore the data.
2. Data Preprocessing
Use the StandardScaler module from scikit-learn to standardize the data.
Create a new DataFrame with the scaled data, using "coin_id" as the index.
3. Finding the Optimal Number of Clusters
Use the Elbow Method to determine the best value for k, examining values from 1 to 11.
Plot the inertia values to visualize the elbow curve and identify the optimal k.
4. Clustering with K-means
Perform clustering using the optimal k value obtained from the Elbow Method.
Create a scatter plot to visualize the clusters using hvPlot.
5. Principal Component Analysis (PCA)
Reduce the dataset's dimensionality to three principal components using PCA.
Analyze the explained variance to understand how much information is retained.
6. Clustering with PCA-Reduced Data
Apply K-means clustering to the PCA-transformed data, using the optimal k value obtained from the Elbow Method.
Create a scatter plot to visualize the clusters, comparing results with those from the original data.
7. Visualization and Comparison
Compare the clustering results of both the original and PCA-reduced datasets using composite plots created with hvPlot.
Repository Contents
Crypto_Clustering.ipynb: Jupyter Notebook containing the project code.
crypto_market_data.csv: The dataset used for analysis.
Requirements
scikit-learn
hvPlot
pandas
numpy
