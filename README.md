# Credit Card Customer Segmentation

K-means clustering to segment customers into VIP, High-Risk, and Low-Risk groups based on spending behavior.

## Key Features
- **Data Preprocessing**: Handled missing values, encoded categorical features, and scaled numerical data.
- **Clustering**: Used K-means (k=3) to identify distinct customer segments.
- **Visualization**: PCA plots and radar charts to highlight segment differences.

## Results
| Segment          | Key Characteristics                     |
|------------------|-----------------------------------------|
| VIP (High-Value) | High credit limits & transaction volume |
| High-Risk        | High utilization, low limits            |
| Low-Risk         | Low utilization, moderate spending      |

## Code Example
```python
from sklearn.cluster import KMeans
kmeans = KMeans(n_clusters=3)
df['Cluster'] = kmeans.fit_predict(scaled_data)
```

## Requirements
- Python 3.8+
- Libraries: pandas, scikit-learn, plotly
