# Supervised Machine Learning- Predicting Credit Risk

![image](https://user-images.githubusercontent.com/99145651/182967222-72f64764-d7bc-4525-970a-0ca010ab1566.png)



## Background

Lending services companies allow individual investors to partially fund personal loans as well as buy and sell notes backing the loans on a secondary market. This data will be used to create machine learning models to classify the risk level of given loans. 

Specifically, comparing 

* Logistic Regression model 
* Random Forest Classifier.

## Instructions

### Retrieve the data

The data is located in the Resources folder.

* `lending_data.csv`

![image](https://user-images.githubusercontent.com/99145651/182967815-d00a96b1-273b-4712-80c2-3f54198ef883.png)


### Import the data using Pandas.

![image](https://user-images.githubusercontent.com/99145651/182968360-dde70006-8c6b-452a-849a-9e0563e2bb53.png)


## Consider the models

#### Create and compare two models on this data: a logistic regression, and a random forests classifier. Prior to creation, fitting, and scoring the models, make a prediction as to which model will perform better. There's no correct response! Write down (in markdown cells in Jupyter Notebook or in a separate document) the prediction, and provide justification for the educated guess.

Let's first look at the meaning of both Logistic Regression and Random Forest Classifier. By definition, Logistic regression is a classification algorithm used to predict a discrete set of classes or categories (e.g., Yes/No, Young/Old, Happy/Sad). This can also be referred to as a binary outcome. In additiona, a logistic regression model predicts a dependent data variable by analyzing the relationship between one or more existing independent variables. Random Forest is a robust machine learning algorithm that can be used for a variety of tasks including regression and classification. It is an ensemble method, meaning that a random forest model is made up of a large number of small decision trees, called estimators, which each produce their own predictions. The random forest model combines the predictions of the estimators to produce a more accurate prediction.

A Logistic Regression usually gives probability associated with each output. It is used to measure the statistical significance of each independent variable with respect to that probability. With Random Forest Clasification, there is further analysis of how a feature contributes to class prediction. Random Forest Classifier also uses decision trees that can capture feature patterns to provide the improved accuracy. These decision trees are used to classify new object from input vector.

Taking this information into account, my prediction is that Logistic regression will be more accurate.

## Fit a LogisticRegression model and RandomForestClassifier model

#### Create a LogisticRegression model, fit it to the data, and print the model's score. Do the same for a RandomForestClassifier. Choose any starting hyperparameters. Which model performed better? How does that compare to the prediction? Write down results and thoughts.

The Logistic Regression performed better than the Random Forest. This supports my prediction that logistic regression analysis would be more accurate. The Training Score was 0.9941188609162196 while the Testing Score came in at 0.9941704498555509. For the Random Forest model, the Training Score was 0.9971970009629936 and the Testing Score equaled 0.991900536524969. The goal of each model was to predict whether a loan would be approved or not. The logistic regression in general, aimed to produce an estimation of the probability of becoming a yes or no. So there is only one "probability" the logistic regression. On the other hand, the probability obtained using random forest can be more like a by product, taking advantage of multiple trees, therefore, could be the potential for different ways to infer the "probabilities" from the model. The does not appear to be overfitting which occurs when machine learning model tries to fit the training data too well. It is usually caused by complicated functions which lead to low error in Training set but high error in Test set called as ‘High Variance’. In conclusion, I'm confident in the Logistic regression because it is easy to implement and interpret.
