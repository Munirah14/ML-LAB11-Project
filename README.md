# ML-LAB11-Project
# Credit Card Customer Segmentation

ARTI308 - Machine Learning | K-Means Clustering Assignment

## Files
- `02-Credit_Card_Customer_Segmentation_Solved.ipynb` — completed notebook
- `CC_GENERAL.csv` — dataset (place in the same folder before running)

## What It Does
Uses K-Means clustering to segment 8,950 credit card customers into **4 groups** based on spending behavior (balance, purchases, cash advance, payments, etc.).

| Cluster | Segment | Description |
|---------|---------|-------------|
| 0 | Regular Shoppers | Moderate balance, active purchases |
| 1 | High-Value Customers | Highest spending and payments |
| 2 | Cash Advance Users | High cash advance, low purchases |
| 3 | Inactive Users | Low balance, minimal activity |

## Key Steps
- Drop `CUST_ID`, fill missing values with column mean
- Scale features with `StandardScaler`
- Choose K using the Elbow Method + Silhouette Score → **K = 4**
- Visualize clusters with PCA (2D)

## Dependencies
```
pandas, numpy, matplotlib, seaborn, scikit-learn
```
