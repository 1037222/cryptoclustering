# CryptoClustering Project

## Overview

Welcome to my CryptoClustering project! In this challenge, I will use my Python skills to apply unsupervised learning techniques and predict whether cryptocurrencies are affected by 24-hour or 7-day price changes. The project involves various tasks, including data preparation, clustering using K-Means, and optimizing clusters through Principal Component Analysis (PCA).

## Project Structure

### Before I Begin

1. **Repository Setup:**
   - I created a new repository for this project called **CryptoClustering**. This homework is not added to an existing repository.
   - I cloned the new repository to my computer.
   - I pushed my changes to GitHub.

2. **Download Files:**
   - I downloaded the [Module 19 Challenge files](#) to help me get started.

### Files

- **Crypto_Clustering.ipynb:** The Jupyter Notebook containing the code for the project.

## Project Tasks

### 1. Data Preparation

- **Load Data:**
  - I loaded the `crypto_market_data.csv` into a Pandas DataFrame.
  - I generated summary statistics and plotted the data to understand its structure.

- **Normalize Data:**
  - I used `StandardScaler` from scikit-learn to normalize the data.
  - I created a DataFrame with the scaled data and set the "coin_id" index from the original DataFrame as the index for the new DataFrame.
  - I displayed the first five rows of the scaled DataFrame.

### 2. Find the Best Value for k Using the Original Scaled DataFrame

- I used the elbow method to find the best value for k.
- I plotted a line chart of inertia values to identify the optimal value for k.
- I answered the question: What is the best value for k?

### 3. Cluster Cryptocurrencies with K-means Using the Original Scaled Data

- I initialized the K-means model with the best value for k.
- I fitted the K-means model using the original scaled DataFrame.
- I predicted the clusters and added a new column to the original data with the predicted clusters.
- I created a scatter plot using hvPlot.

### 4. Optimize Clusters with Principal Component Analysis

- I performed PCA on the original scaled DataFrame and reduced features to three principal components.
- I retrieved the explained variance to determine the total explained variance of the three principal components.
- I created a new DataFrame with the PCA data and set the "coin_id" index from the original DataFrame as the index for the new DataFrame.

### 5. Find the Best Value for k Using the PCA Data

- I used the elbow method on the PCA data to find the best value for k.
- I plotted a line chart of inertia values.
- I answered the questions: What is the best value for k when using the PCA data? Does it differ from the best k value found using the original data?

### 6. Cluster Cryptocurrencies with K-means Using the PCA Data

- I initialized the K-means model with the best value for k.
- I fitted the K-means model using the PCA data.
- I predicted the clusters and added a new column to the PCA data with the predicted clusters.
- I created a scatter plot using hvPlot.

### 7. Visualize and Compare the Results

- I created composite plots to compare elbow curves and cryptocurrency clusters from original data and PCA data.
- I answered the question: Based on visually analyzing the cluster analysis results, what’s the impact of using fewer features to cluster the data using K-means?

## Project Requirements and Grading

The project will be evaluated based on the following criteria:

- **Find the Best Value for k by Using the Original Data (15 points):**
  - I coded the elbow method algorithm to find the best value for k. Used a range from 1 to 11.
  - I plotted a line chart of all the inertia values computed with different values of k.
  - I answered the question: What’s the best value for k?

- **Cluster the Cryptocurrencies with K-Means by Using the Original Data (10 points):**
  - I initialized the K-means model with four clusters using the best value for k.
  - I fitted the K-means model using the original data.
  - I predicted the clusters and reviewed the resulting array of cluster values.
  - I created a scatter plot using hvPlot.

- **Optimize the Clusters with Principal Component Analysis (10 points):**
  - I created a PCA model instance and set `n_components=3`.
  - I used PCA to reduce features to three principal components. Reviewed the first five rows of the DataFrame.
  - I got the explained variance to determine the total explained variance of the three principal components.
  - I created a new DataFrame with the PCA data.

- **Find the Best Value for k by Using the PCA Data (10 points):**
  - I coded the elbow method algorithm and used the PCA data to find the best value for k (range: 1 to 11).
  - I plotted a line chart of inertia values.
  - I answered the questions: What’s the best value for k when using the PCA data? Does it differ from the best k value found using the original data?

- **Cluster the Cryptocurrencies with K-means by Using the PCA Data (10 points):**
  - I initialized the K-means model with four clusters using the best value for k.
  - I fitted the K-means model using the PCA data.
  - I predicted the clusters and reviewed the resulting array of cluster values
