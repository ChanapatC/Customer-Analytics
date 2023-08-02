# Churn scoring

**Notebooks:** [Classification Model](./ChurnScoring.ipynb)  
**Google Colab:** [![Open In Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ChanapatC/Customer-Analytics/blob/main/%234%20Churn%20scoring/Basic_Churn_Prediction.ipynb)

### What's Churn scoring
Churn scoring, also known as customer churn prediction or customer attrition analysis, is a process of using data and analytics to assess the likelihood that a customer will stop doing business with a company or cancel their subscription within a specific period. The term "churn" refers to the rate at which customers leave or "churn out" from a company's customer base.

Here's an overview of how to do churn scoring:

- Data Collection: Gather relevant data about your customers, including historical transaction records, customer interactions, engagement metrics, demographic information, and any other data that may be relevant to customer behavior.
- Data Preprocessing: Clean and prepare the data for analysis. This step involves handling missing values, removing duplicates, and transforming the data into a suitable format for modeling.
- Feature Engineering: Select or create relevant features (variables) that are likely to influence customer churn. These features could include factors such as the frequency of purchases, customer tenure, customer support interactions, customer satisfaction scores, and more.
- Data Splitting: Divide the dataset into two parts: a training set and a test set. The training set is used to build the churn prediction model, while the test set is used to evaluate the model's performance.
- Model Selection: Choose an appropriate machine learning algorithm for churn prediction. Commonly used algorithms include logistic regression, decision trees, random forests, support vector machines, and neural networks. The choice of model depends on the data and the complexity of the problem.
- Model Training: Train the selected model on the training data. The model will learn from historical data to identify patterns associated with customer churn.
- Model Evaluation: Evaluate the trained model's performance using the test dataset. Common evaluation metrics for binary classification problems like churn prediction include accuracy, precision, recall, F1-score, and area under the receiver operating characteristic curve (AUC-ROC).
- Churn Scoring: Use the trained model to predict churn probabilities for each customer in the database. The output of the model will be a churn score or probability indicating the likelihood of a customer churning.
- Set Churn Threshold: Decide on a churn probability threshold above which a customer will be classified as high-risk for churn. This threshold can be adjusted based on the business's risk tolerance and resources for retention efforts.
- Implement Retention Strategies: Based on the churn scores and identified high-risk customers, implement targeted retention strategies, such as personalized offers, loyalty programs, customer outreach, or discounts to reduce the likelihood of churn.
- Monitor and Refine: Continuously monitor the churn prediction model's performance and update it with new data periodically. Refine the model and strategies based on new insights and changes in customer behavior.

Churn scoring is a valuable tool for businesses to proactively address customer attrition and improve customer retention, leading to better customer satisfaction and long-term business success.

# Workshop

## 1) Dataset

The data is a customertravel dataset, the details as below;

Number of observations: 954
Number of variables: 7



## 2) EDA
<img width="409" alt="Screenshot 2023-07-29 at 21 53 43" src="https://github.com/ChanapatC/Customer-Analytics/assets/136244448/2c2b3f95-424a-4171-aace-85aa46a04f7f">

**Create column of average Age and ServicesOpted**

<img width="185" alt="Screenshot 2023-07-30 at 13 02 09" src="https://github.com/ChanapatC/Customer-Analytics/assets/136244448/39971fc6-526b-4da9-bdef-3e0326f43ab4">

***Variable name with types:***

<img width="258" alt="Screenshot 2023-07-30 at 13 03 10" src="https://github.com/ChanapatC/Customer-Analytics/assets/136244448/ed7e7f86-d34b-444b-8f04-8e98da494eb9">

### Summary statistics of numerical variables by Target Flag:

<img width="793" alt="Screenshot 2023-07-30 at 13 04 29" src="https://github.com/ChanapatC/Customer-Analytics/assets/136244448/9d46a0e3-fd36-433b-a343-dc193d93cc0c">

### Multivariate analysis

**Cat-Num**

![image](https://github.com/ChanapatC/Customer-Analytics/assets/136244448/699171c5-a824-4f92-9712-9ca1d7304a11)

![image](https://github.com/ChanapatC/Customer-Analytics/assets/136244448/3b5f9b38-0ac0-4f60-bd9e-8b5364cc6848)

Peform T-TEST and ANOVA

<img width="351" alt="Screenshot 2023-07-30 at 13 08 17" src="https://github.com/ChanapatC/Customer-Analytics/assets/136244448/3f3f31b7-6be8-4af0-a34e-4ea0bb7a3685">

--------------------------------

**Cat-Cat**

![image](https://github.com/ChanapatC/Customer-Analytics/assets/136244448/8683b658-de6c-483b-bf30-0297d814f47f)
![image](https://github.com/ChanapatC/Customer-Analytics/assets/136244448/8974359c-b692-47d9-811d-c4f1e5273117)
![image](https://github.com/ChanapatC/Customer-Analytics/assets/136244448/770d1eff-4c87-4aeb-9c7f-c3df82dda6c1)
![image](https://github.com/ChanapatC/Customer-Analytics/assets/136244448/939a8424-b1f9-4043-9a55-18bc4c1c024f)

<img width="378" alt="Screenshot 2023-07-30 at 13 12 13" src="https://github.com/ChanapatC/Customer-Analytics/assets/136244448/4f480e37-d7af-470f-81a8-23868c77724a">



## 3) Model Creation and Evaluation
- Model Used: 'Logistic Regression', 'Random Forest', 'KNeighbors','XGBoost'
- Fixing Imbalance Technique: none, under sampler, over sampler, SMOTE
- The best performing Model: XGBoost, Sampler: on_Sampler

<img width="470" alt="Screenshot 2023-07-30 at 00 44 41" src="https://github.com/ChanapatC/Customer-Analytics/assets/136244448/13bd2e9a-c952-4ff7-a8f0-7291e7efe464">

### Results
the best performing model is XGBoost, Sampler:no_sampler

### Cinfusion matrix
![image](https://github.com/ChanapatC/Customer-Analytics/assets/136244448/816350a4-6bd8-4c1c-91bc-4518503659f9)

### ROC-AUC
![image](https://github.com/ChanapatC/Customer-Analytics/assets/136244448/1058bf42-4dec-4b8a-b2b3-0b9fc70c74d1)

### Evaluation
![image](https://github.com/ChanapatC/Customer-Analytics/assets/136244448/778534e9-88d8-4023-af26-990ce55822dd)

### Feature importance

![image](https://github.com/ChanapatC/Customer-Analytics/assets/136244448/e96b714a-d23a-4927-993d-6b48489b1da2)

