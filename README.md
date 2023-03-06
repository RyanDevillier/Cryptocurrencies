# Cryptocurrencies
## Overview of the Project
The goal of this project was to use unsupervised learning algorithms, specifically K-Means Clustering, to make predictions on cryptocurrency data.  We used Pandas to preprocess our data so that we could reduce the number of dimensions of our dataset via Principal Component Analysis (PCA).  Once our data was sufficiently prepared, we created an elbow curve using hvPlot.  This elbow curve helped us determine what K value we should use to run our K-Means algorithm with.  Upon determining this K value, we inputted our data into the K-Means algorithm and visualized the clusters with a 3D plot using Plotly Express.  Then, we sliced our data to yield only the cryptocurrencies that were tradable.  This subset of the original data was standardized, cleaned, and then inputted into an hvPlot scatter plot so that we easily visualize our results.    

## Results
As briefly mentioned above, once we preprocessed our initial cryptocurrency data, we plotted this data to create an elbow curve that would allow us to choose the best possible value for K.  Upon doing this, we discovered that the best K value would likely be K = 4, as shown below in the graph of the elbow curve. 
![Elbow_Curve](https://user-images.githubusercontent.com/115128743/223017582-fdc4bd21-8c0f-42f8-a79c-72e449eebcd3.png)


Once we knew the K value we needed, we instantiated a K-Means model and inputted our preprocessed data to yield predictions of the K-clusters for the cryptocurrency data.  After obtaining the K-Means model’s predictions, we concatenated our preprocessed data with the prediction data, and used this concatenation to visualize the clustering of our cryptocurrencies, as shown below.
![Module_19_3D_Plot](https://user-images.githubusercontent.com/115128743/223017590-b2a50105-f89d-4085-94e0-ad7c1a18f881.png)

Finally, we generated a table from the previous dataframes that we used, in addition to hvPlot, to visualize the total number of coins mined vs the total coin supply per cryptocurrency, as shown below.
![Module_19_Scatter_Plot](https://user-images.githubusercontent.com/115128743/223017604-d094c806-3ab0-4b15-b701-7a0d9279dcff.png)
