# 📊 K-Means Clustering: Income vs Age

## 🧠 Description
This project applies **K-Means clustering** to segment individuals based on their **age** and **income**.  
Clusters help identify groups with similar financial and demographic profiles.

---

## 🎯 AIM
To group individuals into clusters based on **Age** and **Income($)** using **K-Means** algorithm, and visualize the clustering results.

---

## 🧩 Goals
- Identify **distinct groups** within the dataset using K-Means.  
- Visualize clusters in **2D and 3D** plots.  
- Scale features using **MinMaxScaler** for better clustering.  
- Analyze cluster centroids and understand the distribution of data.

---

## ⚙️ Technical Details
**Language & Libraries:**  
- Python  
- pandas  
- numpy  
- matplotlib  
- scikit-learn  
- plotly (for interactive 3D visualization)  

---

## 🧾 Data Preprocessing
- Load dataset with `pandas`.  
- Explore data using `.head()` and scatter plots.  
- Scale **Age** and **Income($)** using **MinMaxScaler**.  
- Prepare features for clustering.

---

## 🧮 Model Used
**K-Means Clustering**  
- Number of clusters: `n_clusters=3`.  
- Algorithm assigns each data point to the **nearest cluster centroid**.  
- Centroids updated iteratively until convergence.

---

## 💻 Code Implementation

```python
# Import libraries
import pandas as pd
import numpy as np
from sklearn.preprocessing import MinMaxScaler
from sklearn.cluster import KMeans
import matplotlib.pyplot as plt
%matplotlib inline
import plotly as py
```
📊 Results
Number of clusters: 3

Cluster Centroids (scaled features):

[[0.85294118, 0.2022792],
 [0.1372549 , 0.11633428],
 [0.72268908, 0.8974359]]

📋 Observations

Cluster 0: Younger individuals with lower income.

Cluster 1: Middle-aged individuals with moderate income.

Cluster 2: Older individuals with higher income.

Scaling the features improves clustering performance.

Plotly 3D visualization helps in interactive exploration of clusters.
import plotly.graph_objs as go

