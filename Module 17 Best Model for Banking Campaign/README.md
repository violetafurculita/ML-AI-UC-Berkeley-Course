**Overview:**
In this assignment, our goal is to compare the performance of the classifiers (k-nearest neighbors, logistic regression, decision trees, and support vector machines) we encountered in this section of the program. We will use a dataset related to the marketing of bank products over the telephone.

**Data:**
The dataset used comes from the UCI Machine Learning repository [Links to an external site](https://archive.ics.uci.edu/dataset/222/bank+marketing). The data is from a Portuguese banking institution and is a collection of the results of multiple marketing campaigns. We can make use of the article accompanying the dataset (please see CRISP DM BANK pdf in this folder) for more information on the data and features.

**Deliverables:**
After understanding, preparing, and modeling the data, build a Jupyter Notebook that includes a clear statement demonstrating your understanding of the business problem, a correct and concise interpretation of descriptive and inferential statistics, our findings (including actionable insights), and next steps and recommendations.

[**Jupyter Notebook**](https://github.com/violetafurculita/ML-AI-UC-Berkeley-Course/blob/main/Module%2017%20Best%20Model%20for%20Banking%20Campaign/Module_17_Comparing_Classifiers.ipynb)


**Assignment Solution**

**Disclaimer**

All findings and recommendations are based on only evaluating the 7 features for this assignment. We did not evaluate all features in this original dataset due to model complexity and compute power needed to train and test.

**Problem Statement**

Build and compare machine learning models that can help predict whether a Portuguese banking client will buy or not a term deposit product.

**Our Findings with actionable insights**

Overall the marketing campaigns have a low conversion rate. This means an **8% conversion rate** in this case.

![image](https://github.com/violetafurculita/ML-AI-UC-Berkeley-Course/assets/147281922/f6aa1d0d-e504-4733-ad66-18f1093f4ea0)


The profile of the customer who bought the term deposit product is:

* someone with age between 25-60 years old
  
  ![image](https://github.com/violetafurculita/ML-AI-UC-Berkeley-Course/assets/147281922/0ea18e90-240a-4721-9238-935c66397b39)

* employed as admin, technician or blue-collar

  ![image](https://github.com/violetafurculita/ML-AI-UC-Berkeley-Course/assets/147281922/bec74d63-a3f0-4b2c-8a9f-e2e0eacc1b00)

* someone who either has a high school or university degree

  ![image](https://github.com/violetafurculita/ML-AI-UC-Berkeley-Course/assets/147281922/0f165fa7-8e3a-49c0-aa10-22b2c5afdd59)

* someone who is either married or single

  ![image](https://github.com/violetafurculita/ML-AI-UC-Berkeley-Course/assets/147281922/45c46a4f-9ae1-4f02-9ad1-37b8790415ec)

* someone who does not have a personal loan and if they did in the past, they did not default on the loan
  
  ![image](https://github.com/violetafurculita/ML-AI-UC-Berkeley-Course/assets/147281922/c4a69a7e-63a9-45f6-b752-18b06fb1548a)


  ![image](https://github.com/violetafurculita/ML-AI-UC-Berkeley-Course/assets/147281922/9e757a18-8480-4a61-876e-ed9534a85acc)


* someone who may have a housing loan
  
![image](https://github.com/violetafurculita/ML-AI-UC-Berkeley-Course/assets/147281922/b58cfaee-92fc-4570-9b16-517b6685ec47)

* Best Model to predict propensity to buy by test accuracy and train time - Logistic Regression with a test accuracy of 88.84% and a train time of 0.064. The second best model after fine-tuning is Decision Tree, also based on train time and test accuracy.
* **Before fine-tuning**
  
  ![image](https://github.com/violetafurculita/ML-AI-UC-Berkeley-Course/assets/147281922/e947dcec-306a-4489-aa31-1669788432d6)

* **After fine-tuning and final**
  
  ![image](https://github.com/violetafurculita/ML-AI-UC-Berkeley-Course/assets/147281922/8b697f07-f2ac-4259-b21a-ae7f50595d51)

Evaluating only the **first 7 data features age, type of job, marital status, education level, loan defaults, housing loan status and personal loan status** and not including the rest we still achieved predictive power for our models in high 88th percentiles. Out of those 7 features we further simplified the number of features needed using PCA.

Leveraging combined age, job type, marital status, and education level we can explain 99.99% of the variability in this data set. This means that further adding features to the data set may add incrementally little to no value to our models' ability to predict term deposit purchases.

Applying hyperparameters and finetuning the models produce better accuracy rates for our models. Further fine tuning is possible at the expense of model complexity and compute power needed.
