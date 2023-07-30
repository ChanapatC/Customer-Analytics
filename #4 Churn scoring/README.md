# Churn scoring

**Notebooks:** [Classification Model](./ChurnScoring.ipynb)  
**Google Colab:** [![Open In Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://github.com/ChanapatC/Customer-Analytics/blob/main/%234%20Churn%20scoring/Basic_Churn_Prediction.ipynb)

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

