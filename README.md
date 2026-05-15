# Implementation-of-K-Means-Clustering-for-Customer-Segmentation

## AIM:
To write a program to implement the K Means Clustering for Customer Segmentation.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm:
1. Load customer data and select important features.
2. Choose the number of clusters (K).
3. Run K-Means to group similar customers.
4. Analyze the clusters for customer segmentation.
## Program:
```
/*
Program to implement the K Means Clustering for Customer Segmentation.
Developed by: Ritika S
RegisterNumber:  212225220086
# Simple K-Means Clustering Program for Customer Segmentation

import pandas as pd
import matplotlib.pyplot as plt
from sklearn.cluster import KMeans

data = pd.read_csv("Mall_Customer.csv")

X = data.iloc[:, [3, 4]].values

kmeans = KMeans(n_clusters=5, random_state=0)

y_kmeans = kmeans.fit_predict(X)

plt.scatter(X[:, 0], X[:, 1], c=y_kmeans, s=50)

# Plot centroids
plt.scatter(kmeans.cluster_centers_[:, 0],
            kmeans.cluster_centers_[:, 1],
            s=200,
            marker='X')

# Labels
plt.xlabel("Annual Income")
plt.ylabel("Spending Score")
plt.title("Customer Segmentation using K-Means")

plt.show()
*/
```
## Output:
![K Means Clustering for Customer Segmentation](sam.png)
<img width="963" height="732" alt="Screenshot 2026-05-15 143832" src="https://github.com/user-attachments/assets/0b83e4f7-73ec-4138-acad-e0afd905e7d7" />

## Result:
Thus the program to implement the K Means Clustering for Customer Segmentation is written and verified using python programming.
