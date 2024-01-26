# Cryptocurrency Market Analysis Using k-Means clustering
In this project we tried to cluster cryptocurrencies using machine learning techniques, specialliy K-Means clustering. 
the goal is to identify patterns and group similar crypto currencies based on their market behavior over different time frames.
The analysis is further refined using PCA(Principal Component Analysis)to optimise clustering.

## Technologies Used:
- Python
- Pandas
- Scikit-learn
- Plotly
- hvPlot
- holoviews

## Data Source 
the dataset crypto_market_data.csv (you can find it in Resource folder) which contain price change data over several time frames.

## Process
### Data Preparation
- Loading data, setting index
- Using StandardScaler() to normalize data

### Clustering Analysis

**K-Means clustering on Original Data**
- Using Elbow method to find the optimal number of K(k=4 in original dataset)
- Perform K-Means method using the optimal k
- Visualazed the results and clusters using scatter plots

**PCA Optimization**
- Applied PCA to reduce number of features to 3 principal components.
- Using Elbow method to find the optimal number of clusters(k=4 in reduced dataset)
- Perform K-Means method using the optimal k

  ## Visualization
  Elbow curves for original and PCA-optimized data.
  Scater plots for original and PCA-optimized basedon different fields.
  3D scatter plot using Plotly for PCA- optimized clustering

  ## Results
  - Identified the best value for k both k=4 for original and Pca optimized.
  - PCA optimized simplified the data while while retaining 89.5%of the variance.(total_explained_variance=0.8950)
  - Contributing
