# CryptoCurrency
## 1. Project overview
To use unsupervised machine learning on a set of data, and to figure out if there is anything the data can tell us, i.e trends or other information

## 2. Resources
Jupyter notebook, version 6.3.0
Python version 3.7.10
Input data: `crypto_data.csv`

## 3. Coding Summary
1. Read in the dataset and convert to a DataFrame
2. Filter/Remove some of the columns based on criterias given
3. Convert any text features in the columns by using `.get_dummies` method
4. Use the `StandardScaler.fit_transform()` from step 4 to Standardize and fit the data
5. Reduce the DataFrame to three principal components, by using principal component analysis `PCA(n_components=3)`
