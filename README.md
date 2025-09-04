# Customer Segmentation Project

## Project Overview

This project focuses on customer segmentation using unsupervised machine learning techniques. The main objective is to group customers based on similar behavioral attributes to support strategic decision-making in marketing and customer relationship management.

## Business Context

In a banking context, understanding customer behavior is critical for:
- Personalized product recommendations
- Targeted marketing strategies
- Customer retention efforts
- Resource optimization

By segmenting customers effectively, institutions can develop specific actions for each group rather than applying general strategies across the entire customer base.

## Dataset

The dataset used in this project was synthetically generated in Python to simulate realistic banking scenarios, as no real-world customer data was available. The following features were included for clustering:

- Age
- Total Spending
- Activity Score
- Number of Loans

Other columns such as gender, income level, and region were used for exploratory analysis but not for clustering.

## Technologies and Tools

- Python 3
- Jupyter Notebook
- pandas, numpy (Data manipulation)
- matplotlib, seaborn (Data visualization)
- scikit-learn (Clustering and preprocessing)

## Methodology

1. **Exploratory Data Analysis (EDA)**
   - Data types and missing values checked
   - Distribution visualized using histograms, boxplots, and KDE plots

2. **Data Preprocessing**
   - Outliers examined
   - Numerical features normalized using `StandardScaler`

3. **Clustering**
   - K-Means algorithm implemented
   - Elbow method and Silhouette Score used to determine optimal number of clusters
   - Optimal cluster count determined as 4

4. **Segment Profiling**
   - Each cluster analyzed based on feature averages
   - Descriptive segment names assigned

## Final Segments

| Cluster | Segment Name         | Description                                     |
|---------|----------------------|-------------------------------------------------|
| 0       | Traditional Customers | Loyal customers with low digital interaction    |
| 1       | Passive Spenders      | Low spending and engagement                     |
| 2       | Credit-Focused        | High loan usage, moderate spending              |
| 3       | Digital Actives       | High engagement and spending, tech-savvy users  |

> Note: Segment names were revised based on feedback to reflect behavioral patterns instead of age-based labels. The model considers multiple dimensions beyond just age.

## Evaluation

- Silhouette Score was used to evaluate clustering performance.
- The score ranged between 0.17 and 0.20, which is acceptable for synthetic behavioral data.

## Limitations and Future Work

- Results may vary when applied to real-world banking data.
- Future improvements may include:
  - Testing alternative clustering methods (e.g., Hierarchical, DBSCAN)
  - Incorporating additional features (e.g., channel usage, transaction frequency)
  - Deploying as a web application for business users

## Author

**Sabiha Nur Diler**  
Computer Engineering Student  
Istanbul Arel University  
[GitHub Profile](https://github.com/sabihadiler)