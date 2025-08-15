# Task 7 – Customer Segmentation Using Unsupervised Learning

## Objective
Segment customers based on demographic and behavioral attributes using K-Means clustering to identify distinct groups for targeted marketing strategies.

## Approach
- Loaded the `Mall Customers.csv` dataset and removed the `CustomerID` column as it is not useful for clustering.
- Handled missing values by filling numeric columns with the median and categorical columns with the mode.
- Converted categorical variable `Gender` into numeric values for modeling.
- Conducted Exploratory Data Analysis (EDA) using **seaborn** and **matplotlib**:
  - Distribution of gender, age, income, and spending score.
  - Relationship between income and spending score.
- Scaled numerical features (`Age`, `Annual Income (k$)`, `Spending Score (1-100)`) using StandardScaler.
- Determined the optimal number of clusters using the **Elbow Method** and **Silhouette Score**.
- Applied K-Means clustering with the chosen `k` and visualized clusters using **PCA**.
- Profiled each customer segment and identified patterns in income and spending behavior.

## Results & Insights
- Clear clusters were identified based on income and spending patterns.
- Certain clusters represent high-value customers with high income and high spending scores.
- Other clusters represent budget-conscious customers or low-engagement segments.
- These insights can guide targeted marketing campaigns such as loyalty programs, premium offers, or reactivation strategies.
