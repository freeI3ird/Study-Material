# Doubts
`Any kind of doubts and their solution`
#### ML
1. `Why & How Lasso is better for feature selection and Ridge is better for model training ?`
2. What leads to overfitting high degree of feature variables or too many Parameters ? Andrew Ng said feature variables and Datacamp guy said Parameters ?
   - **Ans**: Both
   - **Causes of Overfitting**
      - Too many Parameters/Features: Too many parameters implies too many corresponding features, when you have so many features, there are higher chances of including features which are not helping in prediction but only adding noise.
      - Too complex model: Means higher order hypothesis which can fit complex curves into data .
      - No. of features/predictors >= no. of data points
3. `R-squared Error ?`
4. Does logistic regression always produces a **Linear Decision Boundary** ?
   - **Ans**: Logistic regression of sklearn is a linear model, its raw model output z = w@X is linear. That's why it always produces Linear Boundary.
5. `Why for gridsearch of parameter 'C' of logistic regression, we use np.logspace(start, end,num, base) as range of values ?`
6. `What is the effect of No. of features/predictors >= no. of data points ?`
7. Why complex models leads to overfitting ?
   - **Ans:** Complex models learn the pecularities of data(very small details, which are specific to that particular data only). This leads to overfitting of model on that data.
8. `Is logistic linear or non-linear ? `
9. `Mathematics behind the L1 for feature selection and why L2 can't be used for feature selection`
10. `How Best Estimator is selected in the GridSearchCV ?`
11. `Multinomial approach for multi-class classification ?`
12. `When to apply transformation log(x) on our features ? or in general when does log transformation is used ?`
13. `Say I have two features x1 and x2, initially not able to see any relationship between them, then I applied transformation, new features f(x1) and f(x2) now these features have some relationship(say linear etc). How to decide which transformation to apply ?`
14. `What, When, Why and how of drop out layer?`
15. `What, When, Why and how of momentum and decay ?`
16. `Keras Sequential model: In model.fit(features, labels, validation_split = 0.25), why we need a validation set while training, while fitting the model, do we use training loss to adjust parameters or the validation_loss ?`
17. `What is ROC curve and AUC ?`
18. `Naive Bayes works well for NLP task, why is so ?`
#### Coding
1. What is cartesian tree?


#### Python
1. What is context manager in python ?
2. What are decoratores ?
