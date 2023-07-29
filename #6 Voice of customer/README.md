# Voice of customer analytics
### What's VoC?

Voice of Customer (VoC) analytics involves collecting and analyzing customer feedback to understand their preferences and needs. It includes methods like surveys, social media listening, reviews, NPS, and text analytics. The insights help businesses improve products and services, leading to higher customer satisfaction and loyalty.

### These are benefits from doing VoC

1. **Customer-Centric Approach**: VoC analytics helps companies become more customer-centric by gaining direct insights into customer preferences, pain points, and expectations.
2. **Improved Product/Service Development**: Understanding customer feedback allows businesses to make data-driven decisions for product and service improvements, leading to offerings that better meet customer needs.
3. **Enhanced Customer Experience**: By addressing customer concerns and feedback, companies can improve the overall customer experience, leading to higher satisfaction and loyalty.
4. **Increased Customer Retention**: Satisfied customers are more likely to stay loyal to a brand, reducing customer churn and improving customer retention rates.
5. **Better Decision-Making**: VoC analytics provides valuable data to support decision-making processes, helping prioritize initiatives and allocate resources effectively.
6. **Competitive Advantag**e: Companies that actively listen to their customers and act on feedback gain a competitive advantage by offering products and services that align with customer expectations.
7. **Innovation and Differentiation**: VoC insights can inspire innovation and help businesses differentiate their offerings from competitors based on customer preferences.
8. **Reduced Costs**: Addressing customer issues proactively can lead to fewer complaints, returns, and support requests, ultimately reducing operational costs.
9. **Positive Brand Perception**: Responding to customer feedback and implementing improvements demonstrates that the company values its customers, leading to a positive brand perception.
10. **Word-of-Mouth and Referrals**: Satisfied customers are more likely to recommend the company to others, leading to organic growth through positive word-of-mouth and referrals.


# Workshop:Topic modeling with LDA
* *LDA is Latent Dirichlet Allocation algorithm*
  
**Google Colab:** [![Open In Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/jane-russ/MADT8101/blob/main/5.Segmentation/V2_1_HDI_Segmentation.ipynb)

### Objective
Need to know feedback from Youtube-users who intesting on movie name 'OPPENHEIMER'
* *comment source:https://youtu.be/XtPZ8-fjTGQ*

### 1. Create data set
Selecting a random comment from this VDO as a sample for the LDA model.

column name as below;
1) review_id / customer_id / user_id
2) review / comment

<img width="1000" alt="Screenshot 2023-07-28 at 14 15 03" src="https://github.com/ChanapatC/Customer-Analytics/assets/136244448/fd911606-014f-4c17-85b1-4c39e0cef602">


### 2. LDA
**Google Colab:** [![Open In Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/jane-russ/MADT8101/blob/main/5.Segmentation/V2_1_HDI_Segmentation.ipynb)


**Tokenize words with pythainlp**

<img width="596" alt="Screenshot 2023-07-29 at 13 51 09" src="https://github.com/ChanapatC/Customer-Analytics/assets/136244448/22f1c245-bb1d-4903-89ab-aecf48fefe6a">

**Create dictionary**

<img width="697" alt="Screenshot 2023-07-29 at 14 22 24" src="https://github.com/ChanapatC/Customer-Analytics/assets/136244448/21f87d64-1848-4f37-9d3e-d7410d1f6287">

**Topic modeling**

<img width="680" alt="Screenshot 2023-07-29 at 14 23 37" src="https://github.com/ChanapatC/Customer-Analytics/assets/136244448/1a7f9457-e195-45e1-a0c2-381c3373e539">

**Visualizing results**

<img width="915" alt="Screenshot 2023-07-29 at 14 26 13" src="https://github.com/ChanapatC/Customer-Analytics/assets/136244448/44870a32-9eaa-49f0-bd59-2ed438cfd52f">

**Predict topics**

<img width="184" alt="Screenshot 2023-07-29 at 14 27 28" src="https://github.com/ChanapatC/Customer-Analytics/assets/136244448/a2d19de9-8ebf-4c9c-a287-437cc30397bd">
<img width="718" alt="Screenshot 2023-07-29 at 14 27 38" src="https://github.com/ChanapatC/Customer-Analytics/assets/136244448/e3ac4ab6-d360-4a2e-b285-2d592d453dc3">




