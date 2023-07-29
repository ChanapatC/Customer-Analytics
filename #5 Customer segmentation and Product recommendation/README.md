# Customer Segmentation & Segment Movement Analysis

### Business overview of HDI
HDI was established in 1986 by Mr. Peter Chia. HDI became the pioneer in developing the network marketing business in Asia. Since then, millions of individuals were given an opportunity to strive for a better life for them and for their families. He has expanded his market to many countries such as Singapore, Malaysia, Indonesia, Hong Kong and Philippines. HDI have 5 main product categories which are adult and kid, personal care, skincare, food and beverages.

## 1) Import Dataset

**Provided Dataset**
- Data member: master data of downline and their sponsor
- trasaction 2021-2023: sales by bill (json file)

## 2) Data Preparation

1. Cleansing data

*Google Colab:*
[![Open In Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ChanapatC/Customer-Analytics/blob/main/clean_jason.ipynb)

2. Create product master table
   - by SKU
   - create price per unit
3. Join transaction table with product master table and validate sales data each year.

4. List of SCV features

<img width="445" alt="Clustering_Feature" src="https://github.com/ChanapatC/Customer-Analytics/assets/136244448/6ee41614-3d5a-41d6-923b-29bf6c2a14af">


## 3) Clustering

*Google Colab:*
[![Open In Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ChanapatC/Customer-Analytics/blob/main/workshop5_main_clustering.ipynb)

### Choosing K number of clustering
Choose **K=4**

![image](https://github.com/ChanapatC/Customer-Analytics/assets/136244448/bcf61167-3f23-4a12-8b45-7c8023a78997)



### Clustering Result

<img width="384" alt="Screenshot 2023-07-29 at 17 52 22" src="https://github.com/ChanapatC/Customer-Analytics/assets/136244448/b8553951-86e8-4d42-95b6-34ec19d2bd13">



### Feature importance
With the cluster lables as classes to predict, create a Random Forest Classifier 

<img width="531" alt="Screenshot 2023-07-29 at 18 03 23" src="https://github.com/ChanapatC/Customer-Analytics/assets/136244448/1210baed-8c39-48ac-b14c-78a5937dc93b">



*Choosing top 8 rank importance socre, see the proportion of feature importance in each cluster* 

 ![MicrosoftTeams-image (17)](https://github.com/ChanapatC/Customer-Analytics/assets/136244448/30d08766-8e32-48f9-9189-325bf9963617)

## 4)Interpreting Resulys

### Clustering Characteristics
name cluster;
- Cluster 0 = Major major
- Cluster 1 = New star
- Cluster 2 = Survivor
- Cluster 3 = Passive incomer
- Cluster 4 = Lovely introductor

<img width="614" alt="Screenshot 2023-07-29 at 18 05 57" src="https://github.com/ChanapatC/Customer-Analytics/assets/136244448/6f8aecda-1d02-437b-8bf7-30c3cc48184a">


### Business Strategies Recommendation
<img width="619" alt="Screenshot 2023-07-29 at 18 13 05" src="https://github.com/ChanapatC/Customer-Analytics/assets/136244448/c44f89ef-e143-4211-9f8f-5600e817d833">

 
### Further step
- Doing Social network analysis; for getting relationship or downline and upline such as sales volume, similarity of product categories and etc.
- silhouette analysis; it's better than k-median
- separate sales channel analysis; clustering in order to sperate offline and online sales
