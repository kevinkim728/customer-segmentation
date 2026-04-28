# Customer Segmentation

A machine learning project that applies k-means clustering to segment restaurant customers based on purchase behavior, informing targeted marketing strategy.

## Overview

Built a customer segmentation model using synthetic data generated from real business knowledge gained from managing a restaurant. Since actual customer transaction data was not available, I created a realistic dataset based on known pricing, visit patterns, and customer behavior observed during operations.

## Tools & Libraries
- Python
- Pandas
- Scikit-learn (KMeans, StandardScaler)
- Matplotlib

## Data
- 7,121 synthetic customers based on real business knowledge
- Features: customer ID, visit frequency, average spend, time of visit, day preference
- Annual revenue validated against real historical revenue
- 3 customer segments: Regular, Casual, Infrequent

## Methodology
- Generated realistic synthetic data grounded in actual menu prices and observed customer behavior
- Used the elbow method to validate k=3 as the optimal number of clusters
- Clustered on visit frequency as the primary behavioral differentiator
- Used spend and time of visit as descriptive features to interpret each cluster

## Results

| Segment | Customers | Avg Visits/Year | Avg Spend | Revenue % |
|---------|-----------|-----------------|-----------|-----------|
| Regular | 984 | 18.4 | $17.55 | ~45% |
| Casual | 1,719 | 6.4 | $19.42 | ~30% |
| Infrequent | 4,418 | 2.2 | $23.49 | ~25% |

## Marketing Insights
- **Regulars** — loyalty rewards program (visit based)
- **Casual** — frequency incentives to increase visit rate
- **Infrequent** — spend based rewards to capitalize on higher per visit spend

## How to Run
1. Clone the repository
2. Install dependencies: `pip install scikit-learn pandas matplotlib`
3. Open `customer_segmentation.ipynb` in Jupyter or VS Code
4. Run all cells