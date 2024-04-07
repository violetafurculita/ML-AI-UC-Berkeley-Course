**Project Title - Use Machine Learning Models to help predict credit card payments default**
Violeta Furculita

**Executive summary**
Predicting Credit Card Payment Defaults: The Need for High Accuracy Machine Learning Models

- [As reported by the New York Fed](https://www.cnbc.com/2024/02/06/credit-card-delinquencies-surged-in-2023-indicating-financial-stress-new-york-fed-says.html#:~:text=Economy-,Credit%20card%20delinquencies%20surged%20in%202023%2C%20indicating%20'financial,stress%2C'%20New%20York%20Fed%20says&text=Credit%20card%20delinquencies%20surged%20more,New%20York%20Fed%20reported%20Tuesday), credit card delinquency rates surged over 50% in 2023, indicating growing financial stress among consumers. Total U.S. household debt also rose to $17.5 trillion, with credit card balances increasing sharply.

- For financial institutions, higher default rates translate directly to lost revenue, increased collection expenses and damage to balance sheets. Even small increases in defaults across large portfolios can result in substantial losses.

- Traditional tools like FICO scores are lagging indicators that do not capture changing repayment behaviors in a rising rate environment. Forward-looking predictive models are needed to preempt defaults through targeted interventions.

- Machine learning approaches can discover complex patterns across thousands of customer attributes. Models that accurately predict defaults 1-3 statements in advance allow contact of at-risk accounts with customized offers or counseling to improve outcomes.

- By reducing defaults, financial institutions can mitigate risks, optimize underwriting, and safeguard profits during periods of economic stress. Machine learning therefore offers a strategic solution to stay ahead of default trends, protect profits, and strengthen customer relationships.

- Accurate predictive models are more important than ever for credit risk management. This underscores the need for further developing and implementing advanced analytical capabilities.

Rationale
**Context**:

- Credit cards are lines of credit extended to customers to use for everyday purchases
- Most customers make monthly payments toward the principal and interest charged, where applicable. Some customers may forgo making payments due to financial distress or intent to commit fraud
- Credit cards are a major revenue stream for financial institutions
- Even small increases in default rates can lead to significant losses
- Being able to accurately predict which customers may default allows targeted risk management

**Problem:**

- Conventional methods of predicting the likelihood of default at underwriting or during usage may not be well-equipped to predict default
- Identifying at-risk customers early allows contact and/or appropriate loss management
- However, default risk depends on complex interactions of many customer attributes

**Research Question**
Can Machine Learning models accurately predict whether credit card customers will default on their payments?

**Data Sources**
UC Irvine Machine Learning Repository

**Methodology**
- Preprocessing of data
- Feature selection and extraction for model training
- Split data into train and test datasets
- Build a baseline model
- Build, train, and test a couple of different models to determine the best model to predict the default of credit card payments
- Fine-tune the selected model to increase accuracy rates

**Results**
We have further fine-tuned the models run before in Module 20 and have achieved the following results.

  ![image](https://github.com/violetafurculita/ML-AI-UC-Berkeley-Course/assets/147281922/e189c96f-d7de-48bd-8859-f8d680ac2978)
  ![image](https://github.com/violetafurculita/ML-AI-UC-Berkeley-Course/assets/147281922/92bbf941-bd0e-4da8-b9cd-74b6807dcd99)

- Now that we built and selected the best model to recommend to our clients, we will summarize our learnings and findings to our clients and share any next steps.
- **Data Used**

      - For this exercise, we used the following data on users:
      
      - history of last 6 months of payments amounts
      
      - history of last 6 monthly statements balance
      
      - whether they defaulted on their last payment
      
      - credit balance on the account
      
      - demographic data such as age, education level, gender

**Learnings from data**

  - Based on the data analyzed, this credit card company experiences a 22% default rate on credit card payments. This tends to be high. The credit card company needs to further explore ways to reduce this rate.
  
  - The majority of clients are ages 29-45 and most of them have credit limits under 100k. Also under $100k credit limit is where most defaults occur.The credit card company needs to explore its underwriting processes and see if enhancements can be made based on these learnings.
  
  - Surprisingly users with higher level education are defaulting more than the others but also these users are granted credit limits above 200k. The credit card company may consider looking at this segment's behavior in addition to other data points it may have on them such as income, employment status, categories where credit is spent, and asset level...
  
  - Advanced age users with ages greater than 60 and credit limits greater than 200k had a higher propensity of defaulting.
  
  - This data did not contain information on users' recent income, asset levels, categories of goods and services where most of the spending occurs, underwriting credit card limits, or further increases or decreases on credit card limits. These and more can be data points that can further enhance a model's ability to make default predictions.
  
  - We can use supervised machine learning models to train and test their accuracy just on the data available. Even with limited data categories we were able to achieve test scores in 82%.

**Learnings from model training and testing**

  - Models used achieved good performance without much hyper-tuning. This is important as the company can use "out of the box" models to help it predict default rates with pretty high accuracy.
  - The credit card company can consider optimizing for test accuracy and train time combined. While there may be models such as KNN and SVM that can offer higher prediction rates, they are slow and resource-intensive to train as seen above in the train time column of the results table.
  - In addition to using prediction from models the credit card company can use this information in conjunction to other methods of reducing losses they may already employ.
  - Data from these models can spearhead actions such as:
    - outreach campaign to users
    - credit usage counseling
    - payment plans
- Likely the credit card company retains more data on its users, or if it does not it is recommended they do. Some potentially valuable information for further training these models was mentioned above.

  
Link to Business Presentation
[Link to notebook](https://github.com/violetafurculita/ML-AI-UC-Berkeley-Course/blob/main/Module%2024%20Capstone%20Project%20Final%20Report/Capstone_Project_Credit_Card_Default_Payments.ipynb)

