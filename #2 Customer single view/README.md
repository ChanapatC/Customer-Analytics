# Customer Single View (CSV)

## What is CSV?
An accessible and consistent set of information about how a customer has interacted with your company,
including what they have bought, their personal data, opinions and feedback.

The centralized database that consolidates a customer's information and interactions across all business touchpoints. It provides a 360-degree view of the customer, enabling better customer experiences, personalized interactions, and improved relationship management. Businesses can use it to anticipate needs, resolve issues, and tailor marketing efforts effectively.

## The benefits of having a single customer view?
The single customer view should sit at the heart of your business. It gives all departments valuable information to improve their performance. Executives, for example, have more accurate data to make decisions, marketers to deliver more profitable campaigns, and customer support agents to solve issues faster.

## The Key Elements Of Customer Single View

1. Identity Information: Basic demographic details of the customer, such as name, address, contact information, and unique identifiers.
2. Interaction History: A comprehensive record of all interactions between the customer and the business across various channels, including purchases, customer service interactions, website visits, and social media engagements.
3. Transactional Data: Information related to the customer's past purchases, transaction amounts, order history, and payment details.
4. Communication Preferences: Data on the customer's preferred communication channels and frequency of engagement.
5. Social Media Activity: Insights from the customer's interactions on social media platforms, including sentiment analysis.
6. Customer Service Records: Details of customer inquiries, complaints, and resolutions.
7. Loyalty Program Data: Participation in loyalty programs, rewards earned, and redemption history.
8. Marketing Engagement: Data on the customer's responses to marketing campaigns and promotions.
9. Website and App Behavior: Information about the customer's behavior while interacting with the company's website or mobile applications.

![image](https://github.com/ChanapatC/Customer-Analytics/assets/136244448/0fc52fcc-e3ee-4547-bc92-05370a8e9821)

# Wotkshop
**Google Colab:** [![Open In Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ChanapatC/Customer-Analytics/blob/main/03_04_Supermarket_ver2.ipynb)


## 1. Import Data
name's 'supermarket.csv'

![Screenshot 2023-08-02 at 16 11 51](https://github.com/ChanapatC/Customer-Analytics/assets/136244448/18404899-5dfe-45e7-9f10-17bedd0ec5cb)

![Screenshot 2023-08-02 at 16 13 10](https://github.com/ChanapatC/Customer-Analytics/assets/136244448/1553c8f8-1594-4f3c-af83-5a686a0cc690)

## 2. EDA

**Distinct count of BASKET_ID: 77234**

**Create new Column**
- spend_sum_user
- average_spending
- purchase_count
- visit_frequency
- ARPU

**Drop unnecessary features**
- ['SHOP_WEEK', 'SHOP_WEEKDAY', 'SHOP_HOUR','PROD_CODE_10','PROD_CODE_20','PROD_CODE_30',
'PROD_CODE_40','CUST_PRICE_SENSITIVITY','CUST_LIFESTAGE','BASKET_SIZE','BASKET_PRICE_SENSITIVITY','BASKET_TYPE','STORE_CODE','STORE_FORMAT','STORE_REGION']


### Data Frame
![Screenshot 2023-08-02 at 16 22 42](https://github.com/ChanapatC/Customer-Analytics/assets/136244448/920fe79b-36fc-4172-91b3-ee7c8277d8fe)

## 3. Modeling

![image](https://github.com/ChanapatC/Customer-Analytics/assets/136244448/fe5b7b19-fa1b-4700-8ade-8b375f0a4ac4)
**K = 4**

![image](https://github.com/ChanapatC/Customer-Analytics/assets/136244448/5b63d1e1-10df-42f4-b826-d4d46b0bf81b)

### Box plots for each column in each cluster

![Screenshot 2023-08-02 at 16 25 25](https://github.com/ChanapatC/Customer-Analytics/assets/136244448/ccb5b359-cb60-4ff1-8c85-3cf92b4e62f6)
![Screenshot 2023-08-02 at 16 25 36](https://github.com/ChanapatC/Customer-Analytics/assets/136244448/fb52af6b-ad24-4636-8942-a8b9ba9732f5)
![Screenshot 2023-08-02 at 16 25 43](https://github.com/ChanapatC/Customer-Analytics/assets/136244448/7f10b328-ac80-40d9-a38a-88ce5841454c)






