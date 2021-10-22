# CryptoCurrency
## 1. Project overview
To use unsupervised machine learning on a set of data, and to figure out if there is anything the data can tell us, i.e trends or other information

## 2. Resources
Jupyter notebook, version 6.3.0
Python version 3.7.10
Input data: `crypto_data.csv`

## 3. Coding Summary & Analysis
1. Read in the dataset and convert to a DataFrame
2. Filter/Remove some of the columns based on criterias given
3. Convert any text features in the columns by using `.get_dummies` method
4. Use the `StandardScaler.fit_transform()` from step 4 to Standardize and fit the data

<ins>Deliverable 2: Reducing Data Dimensions Using PCA</ins>

5. Reduce the DataFrame to three principal components, by using principal component analysis `PCA(n_components=3)`
6. Fit the data `.fit_transform()`
7. Transform the PCA data to a DataFrame

<ins>Deliverable 3: Clustering Cryptocurrencies Using K-Means</ins>

8. Create an elbow curve to find the best value for *k*
9. Plot the Elbow Curve using `hvplot`
10. Initialize the k-mean model `Kmeans` and `n_cluster=4`
11. Fit the model `model.fit`
12. Predict the clusters `model.predict`
13. Create a new DataFrame including predicted clusters and cryptocurrencies features

<ins> Deliverable 4: Visualizing Cryptocurrencies Results</ins>

14. Creating a 3D-Scatter with the PCA data and the clusters `px.scatter_3d`
15. Create a table with all the currently tradable cryptocurrencies using `hvplot.table()`
16. Use the `MinMaxScaler().fit_transform` method to scale the columns 'TotalCoinSupply' & 'TotalCoinsMined'
17.  Create a new DataFrame, containing 'TotalCoinSupply', 'TotalCoinsMined', 'CoinName', & 'Class' Columns
18.  Create an `hvplot` scatter plot `.hvplot.scatter` with hover information `hover_cols=['CoinName']`

## 4. Results

Dataframe with cleaned data:

![image](https://user-images.githubusercontent.com/85843030/138482260-e5d5b935-8237-4162-85bf-cd60c882736b.png)



DatFrame showing the 3 principal components PC1,PC2,PC3:

![image](https://user-images.githubusercontent.com/85843030/138498974-9af9ceb2-436d-4e06-a406-a327042662ca.png)



New DataFrame inclusing predicted clusters and cryptocurrency features

![image](https://user-images.githubusercontent.com/85843030/138486490-b334e48e-b72f-48f0-a546-eec8ee55307b.png)



Showing the Elbow Curve Plot:
![bokeh_plot](https://user-images.githubusercontent.com/85843030/138488907-480ded4e-a5f3-4b0f-b149-0673969614d7.png)



Visualizing Cryptocurrencies result:
![newplot (1)](https://user-images.githubusercontent.com/85843030/138488247-bac75980-f00f-4300-9774-f242ecb6c862.png)


Interactive hvplot table

![image](https://user-images.githubusercontent.com/85843030/138497806-56c60406-1d55-4bc6-86c0-8a7985e5a4fc.png)


Scatter plot:
![bokeh_plot (1)](https://user-images.githubusercontent.com/85843030/138498449-abe720d5-ee29-497e-b686-dbc2884da572.png)



