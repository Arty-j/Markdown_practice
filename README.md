# Model Crypto Investments
Ch10
In this Challenge, you’ll combine your financial Python programming skills with the new unsupervised learning skills that you acquired in this module.

The CSV file provided for this challenge contains price change data of cryptocurrencies in different periods.

The steps for this challenge are broken out into the following sections:

Import the Data (provided in the starter code)
Prepare the Data (provided in the starter code)
Find the Best Value for k Using the Original Data
Cluster Cryptocurrencies with K-means Using the Original Data
Optimize Clusters with Principal Component Analysis
Find the Best Value for k Using the PCA Data
Cluster the Cryptocurrencies with K-means Using the PCA Data
Visualize and Compare the Results

## Technologies
This project leverages python 3.7.13 with the following packages:

pandas - For data analysis

hvplot - for data visualizaion

sklearn - for modeling libraries

## Import and Prepare the Data
1. Data is imported from crypto_market_data.csv file located in Resources folder, and transformed to a dataframe using pandas.  
2. The dataframe is diplayed and plotted before using the StandardScaler module from scikit-learn to normalize the file data. 

## Finding best value for k
1. Code is written to use the elbow method algorithm to find the best value for k.
2. Inertia is calculated for each possible k using the KMeans model and scaled dataframe. 
3. A line chart with all the inertia values computed for the different values of k isused to identify the optimal value for k.

## Cluster Cryptocurrencies using KMeans modeling
1. Optimal k for the dataframe computed above is used to cluster the data, fit it to the scaled dataframe
2. A new dataframe "df_market_preditcions' is made with coins associated with a cluster value
3. Scatter plot shows the distribution of the clusters aroune the 24hour percent price change and the 7day percent price change

