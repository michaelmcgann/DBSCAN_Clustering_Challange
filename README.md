# DBSCAN_Clustering_Challange

This was part of a challenge from the Udemy Course "Python for Machine Learning and Data Science"

This project applies the Density-Based Spatial Clustering of Applications with Noise (DBSCAN) algorithm to identify patterns in customer shopping data. The goal of the project is to segment customers based on their spending habits across various product categories.

DBSCAN is an unsupervised machine learning algorithm that works well for data which contains clusters of similar density. Unlike K-Means clustering, DBSCAN does not require the user to specify the number of clusters and can identify outliers as noise.

In this analysis, we first preprocess the data by normalizing the features using StandardScaler, ensuring that the spending amounts on different categories are on the same scale.

We then apply the DBSCAN algorithm to this preprocessed data. The model parameters, epsilon (eps), which determines the maximum distance between two samples for them to be considered in the same neighborhood, and minimum samples, the number of samples in a neighborhood for a point to be considered as a core point, were set based on exploratory analysis of the data.

Post clustering, we explore the characteristics of each cluster and the outliers by comparing their statistical properties. This provides insights into the typical shopping patterns within each cluster and those of the outliers.

Finally, the spending means of each cluster are visualized using a heatmap after normalizing the values between 0 and 1 using MinMaxScaler.

This project showcases how DBSCAN can be used for customer segmentation, helping businesses understand customer behavior and enabling them to make informed decisions for targeted marketing, product placement, and other business strategies.
