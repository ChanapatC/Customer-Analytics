# Voice of customer analytics
### What's VoC?

Voice of Customer (VoC) analytics involves collecting and analyzing customer feedback to understand their preferences and needs. It includes methods like surveys, social media listening, reviews, NPS, and text analytics. The insights help businesses improve products and services, leading to higher customer satisfaction and loyalty.

### These are benefits from doing VoC

1. **Customer-Centric Approach**: VoC analytics helps companies become more customer-centric by gaining direct insights into customer preferences, pain points, and expectations.
2. **Improved Product/Service Development**: Understanding customer feedback allows businesses to make data-driven decisions for product and service improvements, leading to offerings that better meet customer needs.
3. **Enhanced Customer Experience**: By addressing customer concerns and feedback, companies can improve the overall customer experience,leading to higher satisfaction and loyalty.
4. **Increased Customer Retention**: Satisfied customers are more likely to stay loyal to a brand, reducing customer churn and improving customer retention rates.
5. **Better Decision-Making**: VoC analytics provides valuable data to support decision-making processes, helping prioritize initiatives and allocate resources effectively.
6. **Competitive Advantag**e: Companies that actively listen to their customers and act on feedback gain a competitive advantage by offering products and services that align with customer expectations.
7. **Innovation and Differentiation**: VoC insights can inspire innovation and help businesses differentiate their offerings from competitors based on customer preferences.
8. **Reduced Costs**: Addressing customer issues proactively can lead to fewer complaints, returns, and support requests, ultimately reducing operational costs.
9. **Positive Brand Perception**: Responding to customer feedback and implementing improvements demonstrates that the company values its customers, leading to a positive brand perception.
10. **Word-of-Mouth and Referrals**: Satisfied customers are more likely to recommend the company to others, leading to organic growth through positive word-of-mouth and referrals.


# Workshop:Topic modeling with LDA
* *LDA is Latent Dirichlet Allocation algorithm*
  
**Google Colab:** [![Open In Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ChanapatC/Customer-Analytics/blob/main/Justdoit_review_opp.ipynb)


### Objective
Need to know feedback from Youtube-users who's intesting on movie name 'OPPENHEIMER'
* *comment source:https://youtu.be/XtPZ8-fjTGQ*

### 1. Create data set
Selecting a random comment from this VDO as a sample for the LDA model.
This Youtube clip is short review name Oppenheimer which is director by Christopher Nolan

column name as below;
1) review_id / customer_id / user_id
2) review / comment

<img width="1000" alt="Screenshot 2023-07-28 at 14 15 03" src="https://github.com/ChanapatC/Customer-Analytics/assets/136244448/fd911606-014f-4c17-85b1-4c39e0cef602">


### 2. LDA
**Google Colab:** [![Open In Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/jane-russ/MADT8101/blob/main/5.Segmentation/V2_1_HDI_Segmentation.ipynb)


**Tokenize words with pythainlp**

<img width="596" alt="Screenshot 2023-07-29 at 13 51 09" src="https://github.com/ChanapatC/Customer-Analytics/assets/136244448/22f1c245-bb1d-4903-89ab-aecf48fefe6a">


**Create dictionary**

<img width="1018" alt="Screenshot 2023-07-29 at 15 11 22" src="https://github.com/ChanapatC/Customer-Analytics/assets/136244448/0a6a9014-1705-4ce3-ba52-857f077d879e">


**Topic modeling**

<img width="685" alt="Screenshot 2023-07-29 at 15 11 45" src="https://github.com/ChanapatC/Customer-Analytics/assets/136244448/2c0467f5-83d4-46da-99c1-2cc7290173b7">



**Visualizing results**

<img width="900" alt="Screenshot 2023-07-29 at 15 12 09" src="https://github.com/ChanapatC/Customer-Analytics/assets/136244448/f2cf34f4-7b0d-4cd3-a35e-05e1239ed5b9">

**Grouping comment topic and score**

<img width="689" alt="Screenshot 2023-07-29 at 15 22 39" src="https://github.com/ChanapatC/Customer-Analytics/assets/136244448/4b5ba8dd-e4a0-4f37-a7c2-e7a1834564d0">


**Predict topics**

<img width="162" alt="Screenshot 2023-07-29 at 15 12 17" src="https://github.com/ChanapatC/Customer-Analytics/assets/136244448/6fd8b8c7-955d-4a4e-bfbc-125ca5f0e624">
<img width="486" alt="Screenshot 2023-07-29 at 15 12 39" src="https://github.com/ChanapatC/Customer-Analytics/assets/136244448/f0fee2be-fa71-45de-b19a-4c0db98bfbdb">





