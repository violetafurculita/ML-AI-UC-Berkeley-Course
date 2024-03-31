**Overview:**
In this assignment, our goal is to compare the performance of the classifiers (k-nearest neighbors, logistic regression, decision trees, and support vector machines) we encountered in this section of the program. We will use a dataset related to the marketing of bank products over the telephone.

**Data:**
The dataset used comes from the UCI Machine Learning repository [Links to an external site](https://archive.ics.uci.edu/dataset/222/bank+marketing). The data is from a Portuguese banking institution and is a collection of the results of multiple marketing campaigns. We can make use of the article accompanying the dataset (in the .zip file) for more information on the data and features.

**Deliverables:**
After understanding, preparing, and modeling the data, build a Jupyter Notebook that includes a clear statement demonstrating your understanding of the business problem, a correct and concise interpretation of descriptive and inferential statistics, our findings (including actionable insights), and next steps and recommendations.

**Jupyter Notebook -> 


**Assignment Solution**

**Disclaimer**

All findings and recommendations are based on only evaluating the 7 features for this assignment. We did not evaluate all features in this original dataset due to model complexity and compute power needed to train and test.

**Problem Statement**

Build and compare machine learning models that can help predict whether a Portuguese banking client will buy or not a term deposit product.

**Our Findings with actionable insights**

Overall the marketing campaigns have a low conversion rate. This means a 5% conversion rate in this case.

The profile of the customer who bought the term deposit product is:

* someone with age between 25-60 years old
* employed as admin, technician or blue-collar
* someone who either has a high school or university degree
* someone who is either married or single
* someone who does not have a personal loan
* someone who may have a housing loan

Best Model to predict propensity to buy by test accuracy and train time -

Evaluating only the first 7 data features age, type of job, marital status, education level, loan defaults, housing loan status and personal loan status and not including the rest we still achieved predictive power for our models in high 80th percentiles. Out of those 7 features we further simplified the number of features needed using PCA.

Leveraging combined age, job type, marital status, and education level we can explain 99.99% of the variability in this data set. This means that further adding features to the data set may add incrementally little to no value to our models' ability to predict term deposit purchases.

Applying hyperparameters and finetuning the models produce better accuracy rates for our models. Further finetuning is possible at the expense of model complexity and compute power needed.
