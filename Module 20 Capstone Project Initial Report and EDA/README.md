### Project Title - Use Machine Learning Models to help predict credit card payments default


**Violeta Furculita**

#### Executive summary
**Predicting Credit Card Payment Defaults: The Need for High Accuracy Machine Learning Models**

- [As reported by the New York Fed](https://www.cnbc.com/2024/02/06/credit-card-delinquencies-surged-in-2023-indicating-financial-stress-new-york-fed-says.html#:~:text=Economy-,Credit%20card%20delinquencies%20surged%20in%202023%2C%20indicating%20'financial,stress%2C'%20New%20York%20Fed%20says&text=Credit%20card%20delinquencies%20surged%20more,New%20York%20Fed%20reported%20Tuesday), credit card delinquency rates surged over 50% in 2023, indicating growing financial stress among consumers. Total U.S. household debt also rose to $17.5 trillion, with credit card balances increasing sharply.

- For financial institutions, higher default rates translate directly to lost revenue, increased collection expenses and damage to balance sheets. Even small increases in defaults across large portfolios can result in substantial losses.

- Traditional tools like FICO scores are lagging indicators that do not capture changing repayment behaviors in a rising rate environment. Forward-looking predictive models are needed to preempt defaults through targeted interventions.

- Machine learning approaches can discover complex patterns across thousands of customer attributes. Models that accurately predict defaults 1-3 statements in advance allow contact of at-risk accounts with customized offers or counseling to improve outcomes.

- By reducing defaults, financial institutions can mitigate risks, optimize underwriting, and safeguard profits during periods of economic stress. Machine learning therefore offers a strategic solution to stay ahead of default trends, protect profits, and strengthen customer relationships.

- Accurate predictive models are more important than ever for credit risk management. This underscores the need for further developing and implementing advanced analytical capabilities.

#### Rationale
**Context**:
- Credit cards are lines of credit extended to customers to use for everyday purchases
- Most customers make monthly payments toward the principal and interest charged, where applicable. Some customers may forgo making payments due to financial distress or intent to commit fraud
- Credit cards are a major revenue stream for financial institutions
- Even small increases in default rates can lead to significant losses
- Being able to accurately predict which customers may default allows targeted risk management

**Problem**:
- Conventional methods of predicting the likelihood of default at underwriting or during usage may not be well-equipped to predict default
- Identifying at-risk customers early allows contact and/or appropriate loss management 
- However, default risk depends on complex interactions of many customer attributes

#### Research Question
Can Machine Learning models accurately predict whether credit card customers will default on their payments?

#### Data Sources
[UC Irvine Machine Learning Repository](https://archive.ics.uci.edu/dataset/350/default+of+credit+card+clients)

#### Methodology
* Preprocessing of data
* Feature selection and extraction for model training 
* Split data into train and test datasets
* Build a baseline model
* Build, train, and test a couple of different models to determine the best model to predict the default of credit card payments
* Fine-tune the selected model to increase accuracy rates

#### Results
- We can easily train and test some out-of-the-box models that can offer pretty decent test accuracy rates and train times either on a data set with 10 features or the entire training set

  **Results on out-of-the-box models with 10 features selected via PCA**
    ![image](https://github.com/violetafurculita/ML-AI-UC-Berkeley-Course/assets/147281922/86f57b26-51e2-40f6-9341-60a004775f75)


    **Results on out-of-the-box models on the entire training set**
    ![image](https://github.com/violetafurculita/ML-AI-UC-Berkeley-Course/assets/147281922/24e81c68-84fd-4b53-8775-cb429d7237f4)


- We can further finetune each model to get better model performance

#### Next steps
- perform more modeling and hyper tuning of the models
- look at model ensembles such as boosting to enhance model performance
- determine which customer data features are most useful to building these models so we can optimize for accuracy and train time
- please see the **Module 24 Folder** that contains the completed project with models and stakeholder presentation

#### Outline of project

- [Link to notebook 1]()
- [Link to notebook 2]()
- [Link to notebook 3]()


##### Contact and Further Information
- please see **Module 24 folder** for complete documentation and full notebook.
