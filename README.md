# Cryptocurrencies
## Overview
To expolre Unsupervised Machine Learning. The Model was used to analyze cryptocurrencies data and create clusters of the currencies. These cluster will be used to make an investment portfolio. 
### Purpose
The purpose of the analysis was to explore unsupervised machine learning models using the following:
- SciKit Learn
- Plotly
- hvPlot
- Pandas
- Kmeans
- Elbow Curves
- Hierarchical clustering

### Results
In ordeer to fulfill the analysis request, the data went through several phases to prepare it for the unsupervised machine learning model. 
#### Preprocessing the Data for PCA
1. The data was preprocessed to remove all cryptocurrencies not being traded, any null values, and coins not being mined.

![deliv1 1](https://user-images.githubusercontent.com/105830665/201808263-904a621b-436a-4214-b79b-6dcdc55b85b7.png)

2. The CoinName column was extracted to its on dataframe. 

![deliv1 2](https://user-images.githubusercontent.com/105830665/201808404-ac886b38-f379-4afd-a1a2-302605e41343.png)

3. Get_dummies() was used to create variables for text. 

![deliv1 3](https://user-images.githubusercontent.com/105830665/201808536-25820db4-e891-4d96-b75a-380ee0e0e389.png)

4. The data was standardized using StandardScaler. 

![deliv1 4](https://user-images.githubusercontent.com/105830665/201808676-37a0b222-632e-44f4-af19-b2fcac4bf0e0.png)

#### Reducing Data Using PCA
1. The PCA alogorithm reduced the data and a new dataframe was created with the reduced data. 

![deliv2](https://user-images.githubusercontent.com/105830665/201808899-e09dec8c-aee6-44fd-a122-93c07e439686.png)

#### Clustering using K-Means
1. An elbow curve was used to determine the K value. 

![deliv3 1](https://user-images.githubusercontent.com/105830665/201809223-cd1b5140-809e-43a8-812c-787de75dc153.png)

2. Predictions are made on the data based on the K clusters.

![deliv 3 2](https://user-images.githubusercontent.com/105830665/201809489-bd491441-f7c8-4fb8-be75-ffdef9a7a89b.png)

3. New Dataframe was created merging two dataframes and adding the coinnames. 

![deliv3 3](https://user-images.githubusercontent.com/105830665/201809646-d5afff59-a3e7-4d76-a4e2-a0371079d3c4.png)

#### Visualizing Results
1. A 3D plot was created and each data point has a details. 

![deliv4 1](https://user-images.githubusercontent.com/105830665/201809807-d45b77e2-7214-4388-8e0b-6f8e170ddb91.png)

2. Using hvplot.table(), a table was created with tradable currencies.

![deliv4 2](https://user-images.githubusercontent.com/105830665/201810138-ac42487b-0a39-474c-a76f-368fbf6a792d.png)

3. The total number of tradable currencies are 532. 

![deliv4 3](https://user-images.githubusercontent.com/105830665/201810633-968dd9f7-bf7a-4476-8d9b-178bb402f5c2.png)

4. A new dataframe was created with scaled, clustered, coin name, and class data.

![deliv4 4](https://user-images.githubusercontent.com/105830665/201810854-a6e7f6da-8c83-4047-b49c-fcf1dd028a34.png)

5. A scatter plot was made using hvplot.

![deliv4 5](https://user-images.githubusercontent.com/105830665/201810949-4803efa9-9d66-4750-8c83-3a8cb25c08ca.png)

### Summary
Unsupervised Machine Learning does not give input and output matches like supervised maching learning. The best thing about unsupervised Machine learning is the analyst gets the freedom to choose the number of clusters that best represents the data. 
After writing the code, all cells are running. There are no leak errors. All graphs are displayed. 
