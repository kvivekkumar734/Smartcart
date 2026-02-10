# 🛒 SmartCart — E-Commerce Customer Recommendation System (Unsupervised Learning)

SmartCart is an **unsupervised machine learning project** that performs **customer segmentation** for an e-commerce platform using clustering techniques.  
The goal is to divide customers into meaningful groups (clusters) so that businesses can run **targeted marketing campaigns, personalized offers, and customer recommendations**.

---

##  Project Highlights

- Built a **Customer Recommendation System** using **4 customer clusters**
- Applied **Feature Engineering** to create meaningful customer attributes
- Implemented and compared clustering models:
  - KMeans Clustering
  - Agglomerative (Hierarchical) Clustering
- Used evaluation methods to select the best clustering approach:
  - Elbow Method
  - Silhouette Score
- Created **Cluster Summary** to understand customer behavior
- Built multiple visualizations for analysis and insights:
  - Heatmap
  - Countplot
  - Scatter Plot
  - Pair Plot

---

##  Best Model (Final Selection)

After comparing both clustering approaches using cluster evaluation techniques,  
 **Agglomerative Clustering performed best** and was selected as the final model for customer segmentation.

---

## Algorithms Used

### 1) KMeans Clustering
- Used to segment customers into clusters based on similarity
- Tuned number of clusters using Elbow Method and Silhouette Score

### 2) Agglomerative Clustering (Hierarchical) — Final Model
- Implemented hierarchical clustering and compared results with KMeans
- Selected as the best model based on better cluster separation and interpretability

---

## 📊 Model Evaluation

###  Elbow Method
Used to find the optimal number of clusters (K).

###  Silhouette Score
Used to validate cluster quality and separation.

---

##  Key Features (Feature Engineering)

Performed feature engineering to improve clustering performance, including:
- Total spending / customer purchase behavior
- Web visits and store purchases and catalog purchase
- Customer tenure
- Age and family attributes
- Education and living status indicators

---

##  Cluster Analysis

After clustering, a **cluster summary table** was generated using:

```python
cluster_summary = X.groupby("clusters").mean()
print(cluster_summary)
