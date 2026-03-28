# Customer-Segmentation-ML
This project focuses on segmenting customers into distinct groups based on their demographics, financial attributes, and behavioral patterns using unsupervised machine learning techniques. The objective is to identify meaningful customer segments that can support targeted marketing strategies, customer retention, and business decision-making.

---

## Dataset
- Source: Kaggle Customer Segmentation Dataset :contentReference[oaicite:0]{index=0}  
- Approximately 1,000 customer records  

### Features
- Demographics: age, gender  
- Financial: income, spending_score  
- Behavioral: membership_years, purchase_frequency  
- Transactional: last_purchase_amount  
- Preferences: preferred_category  

---

## Methodology

### Data Preprocessing
- Handled missing values and cleaned inconsistent entries  
- Removed duplicate records and irrelevant columns  
- Standardized data to ensure consistency  

### Feature Transformation
- Applied One-Hot Encoding for categorical variables  
- Applied StandardScaler for numerical features  
- Combined transformed features using ColumnTransformer  

### Optimal Cluster Selection
- Used Elbow Method (WCSS) to determine optimal number of clusters  
- Validated cluster quality using Silhouette Score  

Optimal number of clusters selected: K = 5  

---

## Model Implementation
- Applied K-Means clustering with k-means++ initialization  
- Used multiple initializations (n_init=10) for stability  
- Assigned cluster labels to original dataset for interpretation  

---

## Dimensionality Reduction and Visualization
- Applied Principal Component Analysis (PCA) to reduce dimensionality  
- Visualized clusters in 2D space  
- Used scatter plots and pair plots to analyze feature relationships  

---

## Model Evaluation
Evaluated clustering performance using:

- Silhouette Score (cluster cohesion)  
- Calinski-Harabasz Index (cluster separation)  
- Davies-Bouldin Index (cluster similarity)  

Results indicate well-defined clusters with realistic overlap typical of behavioral data.

---

## Key Customer Segments

1. Brand Champions  
   High spending, long-term loyal customers driving revenue  

2. Young High Spenders  
   High income and aggressive spending behavior, strong future potential  

3. Sleeping Giants  
   High income but low spending, indicating untapped opportunity  

4. Conservative Wealthy  
   High income but cautious spending patterns  

5. Budget Customers  
   Lower income, price-sensitive segment  

---

## Key Insights
- Customer behavior is multi-dimensional and cannot be explained by income alone  
- High-income customers are not necessarily high spenders  
- Loyalty plays a significant role in driving spending behavior  
- Data-driven segmentation enables targeted and efficient marketing strategies  

---

## Tech Stack
- Python  
- Pandas, NumPy  
- Scikit-learn  
- Matplotlib, Seaborn  

---

## Future Improvements
- Explore hierarchical clustering techniques  
- Apply density-based methods such as DBSCAN  
- Incorporate real-time or streaming customer data  
- Deploy segmentation model for production use  

---

## Author
Nitish Bhatt  
BS Data Science and Applications (IIT Madras) + B.Tech Mechanical Engineering (GBPUAT)
