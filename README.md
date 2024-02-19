# PRODIGY_ML_02
ML Internship at [Prodigy InfoTech](https://prodigyinfotech.dev) 

Task - 02
# K-means clustering algorithm to group customers
This repository contains code on K-means clustering algorithm to group customers of a retail store based on their purchase history.
##
## Description:

In the dynamic landscape of retail, understanding customer behavior is paramount for business success. Leveraging the power of machine learning, this project focuses on employing the K-means clustering algorithm to categorize customers of a retail store based on their purchase history. The aim is to uncover meaningful patterns in customer data, allowing the retail store to tailor its strategies for different customer segments.
## Algorithm:

**Step 1: Import Necessary Libraries**
- Import required libraries such as pandas, numpy, matplotlib.pyplot, seaborn, and KMeans from sklearn.

**Step 2: Load and Explore the Data**
- Read the 'Mall_Customers.csv' dataset into a DataFrame (df).
- Display the first few rows of the dataset using `df.head()`.
- Display the shape of the dataset using `df.shape`.
- Display information about the dataset using `df.info()`.

**Step 3: Prepare Data for Clustering**
- Select relevant columns (features) for clustering, typically representing customer behavior. In this case, columns 3 and 4 are selected and stored in the variable 'X'.

**Step 4: Elbow Method for Optimal Cluster Selection**
- Initialize an empty list 'wcss' to store Within-Cluster-Sum-of-Squares.
- Iterate through a range of cluster numbers (1 to 10) using a for loop.
- For each cluster number, fit a KMeans model and calculate the WCSS, then append it to the 'wcss' list.
- Plot an elbow chart to visualize the WCSS values.
- Choose the number of clusters where the decrease in WCSS starts to slow down (the "elbow" point). In this case, it seems to be 5.

**Step 5: Perform K-means Clustering**
- Initialize a KMeans model with the chosen number of clusters (5).
- Fit the model on the data and obtain cluster labels for each data point.

**Step 6: Visualize the Clusters**
- Plot a scatter plot for the customer data points, color-coded by their assigned clusters (Cust 1 to Cust 5).
- Plot the centroids of the clusters in magenta.
- Add a legend to identify each cluster.

**Step 7: Display the Plot**
- Display the final plot.
  
## Usage:
1) Dataset from Kaggle [Mall Customer Segmentation Data](https://www.kaggle.com/datasets/vjchoudhary7/customer-segmentation-tutorial-in-python).
2) Used Jupiter Notebook for Python Coding.

## Techniques:
The following techniques are implemented in this project:
- K-means clustering algorithm
  
