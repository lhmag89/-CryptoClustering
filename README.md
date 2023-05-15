# CryptoClustering

## Analysis

The purpose of this analysis is to use k-means and PCA to cluster cryptocurrencies by their price change. The data contained 41 cryptocurrencies with 7 price change time intervals as the features. StandardScaler was used to prepare the data. Inertia was found for each k cluster to determine optimal k-value for clustering. K-means was used to predict clusters. The clusters were plotted. Then, a PCA model was used on the scaled data to reduce dimensionality to 3. The same clustering analysis was done with the transformed data.

## Results

* Original Scaled Data
  * use k=4 clusters
  * ![image](https://github.com/lhmag89/CryptoClustering/assets/119267098/b9ed07d3-113a-4fe2-a5b8-e3168d59d369)
  * ![image](https://github.com/lhmag89/CryptoClustering/assets/119267098/3c6dade3-3a8a-41e2-ac69-d8cf8932f9f0)

* PCA Transformed Data
  * use k=4 clusters
  * Total Explained Variance Ratio: 0.895
  * ![image](https://github.com/lhmag89/CryptoClustering/assets/119267098/9eb1ee89-4ef6-4fed-8e1c-7f74cf1cb37b)
  * ![image](https://github.com/lhmag89/CryptoClustering/assets/119267098/b10bef3e-7767-4143-b506-b96acd01dc2d)

## Summary

For both methods, k = 4 was chosen as the optimal values for clustering based on the respective elbow curves. The predicted clusters are identical for both methods. The advantage of PCA is reducing dimensionality to reduce the computational load. The total explained variance ratio is 0.895, meaning the three components used for dimensionality reduction account for 89.5% of the variance.

## Technologies
Python, Jupyter, Pandas, hvplot, sklearn, PCA, Kmeans, StandardScaler

## Contributors
Developed by Luis Hernandez Email: lhernandez.mag.89@gmail.com

## License
UC Berkeley Extension Data Analytics Program
