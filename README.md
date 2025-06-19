# Clustering-with-K-Means
 Clustering with K-Mean

 
## 🎯 Objective
Apply unsupervised learning using **K-Means clustering** to group mall customers into meaningful segments based on their demographics and spending behavior.

---

## 🛠️ Tools & Libraries
- Python
- Scikit-learn
- Pandas
- Matplotlib
- Seaborn

---

## 📂 Dataset
**Mall_Customers.csv**  
Includes 200 customer records with the following features:
- CustomerID
- Gender
- Age
- Annual Income (k$)
- Spending Score (1–100)

---

## ✅ Steps Performed

### 1. Preprocessing
- Removed `CustomerID` (irrelevant for clustering).
- Encoded `Gender` as numerical.
- Scaled features using `StandardScaler`.

### 2. Elbow Method
- Used **Within-Cluster-Sum-of-Squares (Inertia)** to identify optimal number of clusters (`K`).
- Found optimal `K = 5`.

### 3. K-Means Clustering
- Applied `KMeans` with 5 clusters.
- Assigned and stored cluster labels.

### 4. Evaluation
- **Silhouette Score** was calculated to measure clustering quality.
- Higher score indicates better cohesion and separation between clusters.

### 5. Visualization
- **PCA** was used to reduce dimensionality to 2D.
- Plotted clusters with color-coding using `seaborn`.

---

## 📊 Results

| Metric            | Value         |
|-------------------|---------------|
| Optimal Clusters  | 5             |
| Silhouette Score  | ~0.55–0.65    |
| Features Used     | Age, Income, Spending Score |


