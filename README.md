# 🛍️ Mall-Customer-Segmentation-Using-K-means-Clustering

This project uses K-Means clustering to segment mall customers based on their income and spending behavior.

## 📁 Dataset

Source: Mall_Customers.csv from Kaggle

Columns:
CustomerID, Gender, Age, Annual Income (k$), Spending Score (1–100)


## 🧠 Feature Selection Strategy

Only selected features were used for clustering. Other columns were retained in the dataset for post-clustering analysis.

Features Used	Silhouette Score

Annual Income, Spending Score	0.55
+ Gender	0.44
+ Age	0.41
All Columns	Lower


> Conclusion: Using only Annual Income and Spending Score produced the most distinct and meaningful clusters.

## ⚙️ Clustering Process



1. Load full dataset


2. Select only Annual Income (k$) and Spending Score (1-100) for clustering

 
3. Standardize features using StandardScaler


4. Determine optimal K using the Elbow Method


5. Fit KMeans with n_clusters=5


6. Assign cluster labels back to original dataset


7. Evaluate using Silhouette Score


8. Visualize clusters (raw features and optional PCA)

   

## 📈 Result Highlights

K = 5 chosen using the Elbow Method

Clusters show clear separation in income vs. spending behavior

Other features like Gender and Age can be used for further analysis after clustering


![kmeans_clusters](https://github.com/user-attachments/assets/83f777f3-d84b-4971-9be9-32c0c3e0845e)


## 📄 Files

mall_kmeans.ipynb

Mall_Customers.csv

README.md




