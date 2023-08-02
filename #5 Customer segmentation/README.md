# Customer Segmentation & Segment Movement Analysis

## Customer Segmentation:
Customer segmentation is a marketing strategy that divides a company's customer base into distinct groups based on specific characteristics or behaviors. It helps businesses better understand their customers, personalize marketing efforts, and improve overall customer satisfaction.

### Principal Component Analysis (PCA):
PCA is a statistical technique used in data analysis to simplify complex datasets by reducing the number of variables while preserving most of the original information. It transforms correlated variables into a set of uncorrelated principal components, making it easier to interpret and visualize the data. PCA is commonly used for dimensionality reduction and pattern recognition tasks.

**The number of principal components to use in a PCA analysis;**
1. Variance Explained: Selecting enough principal components to retain a significant portion of the total variance in the data. A common approach is to retain components that explain a certain percentage (e.g., 80% or 90%) of the total variance.
2. Scree Plot: Using a scree plot to visualize the eigenvalues of the principal components. The "elbow" point on the scree plot indicates a suitable number of components to retain.
3. Interpretability: Choosing principal components that are easy to interpret and align with the underlying characteristics of the data.
4. Application: Considering the number of principal components that are practically useful for the specific analysis or downstream tasks.
 
 it depends on the specific dataset and the objectives of the analysis. In PCA, the number of principal components chosen can vary based on


## Segment Movement Analysis
Segment Movement Analysis is the study of how individual body segments move during activities. It involves analyzing the motion and forces of specific body parts to understand technique, efficiency, and injury risks in sports and other movements. Advanced technology is often used to collect data for this analysis.



# Workshop: HDI 
## Business overview of HDI ![image](https://github.com/ChanapatC/Customer-Analytics/assets/136244448/6078b92f-f9e6-44d1-ba47-926473f9c9fa)

HDI was established in 1986 by Mr. Peter Chia. HDI became the pioneer in developing the network marketing business in Asia. Since then, millions of individuals were given an opportunity to strive for a better life for them and for their families. He has expanded his market to many countries such as Singapore, Malaysia, Indonesia, Hong Kong and Philippines. HDI have 5 main product categories which are adult and kid, personal care, skincare, food and beverages.

## 1) Import Dataset

**Provided Dataset**
- Data member: master data of downline and their sponsor
- trasaction 2021-2023: sales by bill (json file)

## 2) Data Preparation

1. Cleansing data

*Google Colab:*
[![Open In Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ChanapatC/Customer-Analytics/blob/main/%235%20Customer%20segmentation/clean_jason.ipynb)



2. Create product master table
   - by SKU
   - create price per unit
3. Join transaction table with product master table and validate sales data each year.

4. List of SCV features

<img width="445" alt="Clustering_Feature" src="https://github.com/ChanapatC/Customer-Analytics/assets/136244448/6ee41614-3d5a-41d6-923b-29bf6c2a14af">


## 3) Clustering

*Google Colab:*
[![Open In Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ChanapatC/Customer-Analytics/blob/main/%235%20Customer%20segmentation/workshop5_main_clustering.ipynb)


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
