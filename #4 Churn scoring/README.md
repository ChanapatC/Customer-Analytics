# Churn scoring

**Notebooks:** [Classification Model](./ChurnScoring.ipynb)  
**Google Colab:** [![Open In Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/jane-russ/MADT8101/blob/main/4.ChurnScoring/ChurnScoring.ipynb)

## 1) Dataset

The data is a customertravel dataset, the details as below;

Number of observations: 954
Number of variables: 7


Variable name with types:

Age                            int64
FrequentFlyer                 object
AnnualIncomeClass              int64
ServicesOpted                  int64
AccountSyncedToSocialMedia    object
BookedHotelOrNot              object
Target                         int64

## 2) EDA
<img width="409" alt="Screenshot 2023-07-29 at 21 53 43" src="https://github.com/ChanapatC/Customer-Analytics/assets/136244448/2c2b3f95-424a-4171-aace-85aa46a04f7f">

![image](https://github.com/ChanapatC/Customer-Analytics/assets/136244448/91c536cd-5337-4c30-82f2-cde0750441e5)
![image](https://github.com/ChanapatC/Customer-Analytics/assets/136244448/9feee8bd-c0b8-4757-ae2d-d7a9f8f6c2de)



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

### evaluation
![image](https://github.com/ChanapatC/Customer-Analytics/assets/136244448/778534e9-88d8-4023-af26-990ce55822dd)

### Feature importance

![image](https://github.com/ChanapatC/Customer-Analytics/assets/136244448/e96b714a-d23a-4927-993d-6b48489b1da2)

