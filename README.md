# CryptoClustering

The purpose of this code is to use Python and unsupervised learning to predict if cryptocurrencies are affected by 24-hour or 7-day price changes.

Prepare the Data
- Use the StandardScaler() module from scikit-learn to normalize the data from the CSV file.
- Create a DataFrame with the scaled data and set the "coin_id" index from the original DataFrame as the index for the new DataFrame.

Find the Best Value for k Using the Original Scaled DataFrame
- Use the elbow method to find the best value for k.

Cluster Cryptocurrencies with K-means Using the Original Scaled Data
- Cluster the cryptocurrencies for the best value for k on the original scaled data.

Optimize Clusters with Principal Component Analysis
- Using the original scaled DataFrame, perform a PCA and reduce the features to three principal components.
- Retrieve the explained variance to determine how much information can be attributed to each principal component.
- Create a new DataFrame with the PCA data and set the "coin_id" index from the original DataFrame as the index for the new DataFrame.

Find the Best Value for k Using the PCA Data
- Use the elbow method on the PCA data to find the best value for k.

Cluster Cryptocurrencies with K-means Using the PCA Data
- Cluster the cryptocurrencies for the best value for k on the PCA data.

Questions to answer:
- What is the best value for k using both methods?
- What is the total explained variance of the three principal components?
- What is the impact of using fewer features to cluster the data using K-Means?
