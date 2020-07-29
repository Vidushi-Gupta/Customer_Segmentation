# Customer Segmentation using RFM And K-Means
Customer Segmentation has always been an important aspect of handeling businesses related to services or goods. It is through customer segmentation that one realises if they are adopting the **right strategies** and are having happy consumers of their service. 
The following project utilises the **Recency, Frequency and the Monetary Value approach (RFM)** and the unsupervised learning model by clustering using **K-Means**.
This repository contains two .ipynb for the two different methods used.

## Dataset
The dataset used here is the open-source *[online retail]*(https://archive.ics.uci.edu/ml/datasets/Online+Retail) dataset by the **UCI ML repository**. For this project, the sales of Switzerland were considered as it is one of the countries in the world with the highest cost of living. 

## RFM Analysis
The RFM Analysis involves the following parameters:
R: **Recency**- Depicts the number of days passed since the last transaction.
F: **Frequency**- Shows how frequent a customer comes and buys a product.
M: **Monetary Values**- Depicts the total amount spent by that customer.
For the RFM Analysis a RFM Table was constructed.

![RFM table](https://github.com/Vidushi-Gupta/Customer_Segmentation/blob/master/Visualization/RFM%20Table.png)

Post this, the skewness of the data was evaluated

![skew](https://github.com/Vidushi-Gupta/Customer_Segmentation/blob/master/Visualization/skew.png)

The RFM data was divided into quantiles for analysing after which the RFM score was assigned to each of the customers.
The RFM score determined the customer category.
The different categories obtained were visualised using Plotly

![Recency](https://github.com/Vidushi-Gupta/Customer_Segmentation/blob/master/Visualization/Recency.png)

![Frequency](https://github.com/Vidushi-Gupta/Customer_Segmentation/blob/master/Visualization/Frequency.png)

![Monetary Value](https://github.com/Vidushi-Gupta/Customer_Segmentation/blob/master/Visualization/Monetary.png)

A **square plot** was plotted using squarify in order to analyse the segments with respect to a whole picture

![Square plot](https://github.com/Vidushi-Gupta/Customer_Segmentation/blob/master/Visualization/square%20plot%20segments.png)

This clearly shows the count with respect to the total. Thus helping with understanding the effects of the marketing strategies. 
To analyse the count of customers in each segmet, a **bubble plot** was plotted using Plotly

![bubble plot](https://github.com/Vidushi-Gupta/Customer_Segmentation/blob/master/Visualization/bubble%20plot.png)

### Conclusion
The best customers spent a huge amount on online retail buying, were frequent and bought often. However a good amount of customers had less frequency and better marketing strategies like offer emails and discount vouchers should be adopted so that more customers are attracted.


## K Means Clustering
The **Elbow method** was used to identify the appropriate number of clusters for the Switzerland Dataset.

![Elbow](https://github.com/Vidushi-Gupta/Customer_Segmentation/blob/master/Visualization/Elbow%20method.png)

The graph shows that **3 number of clusters** are ideal. This conclusion was derived because the graph takes a steep movement before 3 and becomes linear after it.
Post this, the unsupervised K-means clustering model was fit to the dataset and then the results were visualized in a line plot by the seaborn library.

![Snake Plot](https://github.com/Vidushi-Gupta/Customer_Segmentation/blob/master/Visualization/Snake%20plot.png)

A **dot plot** was plotted using Plotly in order to analyse the count in each cluster of customers.

![dot](https://github.com/Vidushi-Gupta/Customer_Segmentation/blob/master/Visualization/clusters%20dot%20plots.png)

### Conclusion
The Snake plot shows the monetary attribute and concludes that cluster 1 accounts to the best customers.
Cluster 2 shows for the lost customers or churned customers. However, cluster 0 shows potential customers. They can be converted to the best customers by providing them with better incentives to shop.


You're most welcome to use the notebooks attached here or to fork the repository.

Happy Visualizing!
