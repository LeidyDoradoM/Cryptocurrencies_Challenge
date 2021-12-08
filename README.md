# Cryptocurrencies Project

A prominent investment bank is interested in offering a cryptocurrency investment portfolio for its customers.  In this project, we explore available data to get information about the cryptocurrencies that are on the trading market and how they can be classified.

The data used in this project could be find [here](Resources/crypto_data.csv). Since the data does not have known output about categorization of cryptocurrencies, we will use unsupervised learning algorithm: `K-means`, and a pre-processing transformation: `Principal Component Analysis (PCA)`.

## Preprocessing the Data for PCA

Before applying the clustering algorithm, the data needs to be cleaned and prepared. Rows with at least one null value or without coins being mined are removed. As well as, text variables are converted to numerical values (`get_dummies` function), and standardized using the `StandardScaler fit_transform()` function.  Figure 1 shows the DataFrame after applying all the pre-processing:

![data](Images/crypto_df.png)
Figure 1. Cryptocurrences DataFrame

## Reducing Data Dimensions Using PCA

![pca](Images/pcs_df.png)
Figure 2. Principal Components of Cryptocurrences DataFrame

## Clustering Cryptocurrencies Using K-means 

![clustering](Images/clustered_wClasses.png)
Figure 3. Classification of Cryptocurrences DataFrame using the K-means Algorithm

## Visualizing Cryptocurrencies Results


![hvplotT](Images/hvplotTable.png)
Figure 4. Table with Cryptocurrences and Classes

![hvplot](Images/hvScatterPlot.png)
Figure 5. ScatterPlot showing distribution of Cryptocurrences by Classes

## Summary

