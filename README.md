# Default-Credit-Cards
This is the final project for  Artificial Intelligence course, CSCI-6660-01 done by Jayaprakash Dama(00747524), Rajesh kannaboyena(00722139) and Lakshmi Sowjanya Donadri(00746430).

This project involves training a data set with various machine learning techniques and assessing the effectiveness of each model to identify credit card defaulters.

## List of Contents:
+ Data Set </br>
+ Machine Learning models used </br>
+ How we used these models in project</br>
+ Performance</br>

## <a name="Data_Set"  ></a> Data Set 


This dataset includes data on missed payments, demographic factors, credit data, payment history, and bill statements for credit card users from April to September 2005. 

There are 24 features to choose from:

**Demographic Information**
- ID: ID of each client
- LIMIT_BAL: Amount of given credit in NT dollars (includes individual and family / supplementary credit)
- SEX: Gender (1=male, 2=female)
- EDUCATION: (1=graduate school, 2=university, 3=high school, 4=others, 5=unknown, 6=unknown)
- MARRIAGE: Marital status (1=married, 2=single, 3=others)
- AGE: Age in years

**Repayment Status for past 6 months**

**(-1 = pay duly, 1 = payment delay for one month, 2 = payment delay for two months, ..., 9 = payment delay for nine months and above)**
- PAY_0: Repayment status in September, 2005 
- PAY_2: Repayment status in August, 2005 (scale same as above)
- PAY_3: Repayment status in July, 2005 (scale same as above)
- PAY_4: Repayment status in June, 2005 (scale same as above) 
- PAY_5: Repayment status in May, 2005 (scale same as above)
- PAY_6: Repayment status in April, 2005 (scale same as above)

**Amount of bill statement for past 6 months**
- BILL_AMT1: Amount of bill statement in September, 2005 (NT dollar)
- BILL_AMT2: Amount of bill statement in August, 2005 (NT dollar)
- BILL_AMT3: Amount of bill statement in July, 2005 (NT dollar)
- BILL_AMT4: Amount of bill statement in June, 2005 (NT dollar)
- BILL_AMT5: Amount of bill statement in May, 2005 (NT dollar)
- BILL_AMT6: Amount of bill statement in April, 2005 (NT dollar)

**Amount of previous payment for past 6 months**
- PAY_AMT1: Amount of previous payment in September, 2005 (NT dollar)
- PAY_AMT2: Amount of previous payment in August, 2005 (NT dollar)
- PAY_AMT3: Amount of previous payment in July, 2005 (NT dollar)
- PAY_AMT4: Amount of previous payment in June, 2005 (NT dollar)
- PAY_AMT5: Amount of previous payment in May, 2005 (NT dollar)
- PAY_AMT6: Amount of previous payment in April, 2005 (NT dollar)

**Target Variable**
- default payment next month: Default payment (1=yes, 0=no)
***

## <a name="Machine_Learning_models_used"> </a> Machine Learning models used 
**SVM**

Support vector machines (SVMs), a type of supervised machine learning technique, can be used for both classification and regression tasks. However, it is usually used to address categorization issues. Each value in the SVM algorithm at a specific location. For every piece of information, make a point in n-dimensional space (n is the number of features) that symbolizes the feature's value. Find a super plane that distinguishes the two classes clearly, and then classify them.

**How it works**

A straightforward linear SVM classifier operates by tracing a straight line between two classes. In other words, all the data points on one side of the line correspond to a category, whereas the data points on the other side of the line are assigned to different categories. This implies that you can choose from an endless number of lines. The linear SVM algorithm chooses the optimum line for classifying data points, making it preferable than other techniques like closest neighbor. Select a line to divide the data, keeping it as far away from the cabinet data points as you can. If you utilize 2D examples, all machine learning jargon will be simpler to comprehend. A grid usually contains multiple data points. These data points need to be categorized, but you don't want to categorize them wrongly. This indicates that the line separating the other data points from the two closest points is what we're looking for. As a result, the reference vector for identifying this line is provided by the two nearest data points. This line is known as the decision boundary.

**Logistic Regression**

A type of statistical analysis is logistic regression, sometimes known as logit regression, binary logit, or binary logistic regression. A statistical method known as logistic regression uses historical data to forecast the outcome of a dependent variable. It is a type of regression analysis that is frequently applied to binary categorization problems.
The log of the outcome's odds ratio is modelled by logistic regression. A logistic regression model's coefficients are calculated via maximum likelihood estimation. This is since, unlike linear regression, no closed-form solution exists. Regression analysis is a type of predictive modeling technique that is used to determine the relationship between a dependent variable and one or more independent variables.

**How it works**

We fit a "S" shaped logistic function in logistic regression instead of a regression line, which forecasts two maximum values (0 or 1). The logistic function's curve depicts the likelihood of many outcomes, including whether the cells are malignant, whether or not a mouse is obese based on its weight, and other outcomes. Logistic regression is a crucial machine learning technique because it can produce probabilities and classify new data using both continuous and discrete datasets. Observations can be categorized using a variety of types of data using logistic regression, which can also quickly pinpoint the most beneficial parameters for categorization.

**Naive bayes**

To carry out classification tasks, a Naive Bayes classifier, a probabilistic machine learning model, is used. The classifier's foundation is the Bayes theorem.

**How it works**

Using Bayes' theorem, we may determine how likely it is that A will occur if B has already happened. The hypothesis is A, and B is the proof. In this instance, it is assumed that the predictors and features are independent. In other words, the presence of one trait does not affect the other. It is hence referred to as naive.


**Random Forest**

A supervised learning algorithm is random forest. It assembles decision trees, which are frequently trained using the "bagging" method, into a "forest." The fundamental tenet of the bagging approach is that the output is improved by combining several learning models.

Classification and regression problems, which make up most modern machine learning systems, can be resolved using random forest. Let's examine random forest in categorization since it is usually regarded as the foundation of machine learning.

A decision tree or bagging classifier's hyperparameters are relatively comparable to those of a random forest. Thankfully, you can use a random forest's classifier-class rather than combining a decision tree with a bagging classifier. To handle regression jobs with random forest, use the algorithm's regressor. 

The random forest increases the model's randomness as it grows the trees. Instead of focusing on the most important feature when dividing a node, it chooses the best feature from a random selection of features. There is a lot of diversity as a result, which results in a better model.

As a result, the method for dividing a node in random forest only takes a random subset of the features into account. You can further randomize trees by using random thresholds for each feature rather than aiming for the highest feasible thresholds (like a normal decision tree does).


 ## <a name="How_we_used_these_models_in_project"> </a> How we used these models in project
 
 - Performed training on data set.
- Predicting the model by using test data set.
- Evaluated the model by using F1 score,K Fold Cross validation and confusion matrix.
- Testing the trained model with new dataset

## <a name="Performance"> </a> Performance
**Following is the performance of each models used.**

<img src="https://user-images.githubusercontent.com/119881459/207220712-5576cd04-970f-4deb-8fa4-59ef81aab087.png">

<img src="https://user-images.githubusercontent.com/119881459/207221046-11a0cb05-a4ee-4e36-87c0-915e20c5d6d0.png">

