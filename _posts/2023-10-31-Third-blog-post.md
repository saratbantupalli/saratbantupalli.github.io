# Variable Selection for Statistical Models
Selecting variables for building statistical models is an art gained with experience. Understanding the context of the problem (or data) solves a major chunk of the problem of selecting explanatory variables (their transformations and or combinations). Here I discuss how I usually approach the selection of variables for my models and some selection techniques.

## Guiding Principles for Model Selection
Here are some general principles (or axioms in this case) in model selection that can help with variable selection:  
+  The simplest model is the best model, unnecessary predictors decrease the degrees of freedom and can cause collinearity  
+  Exploratory Data Analysis (EDA) is a great resource to check assumptions about explanatory variables
+  Lower-order terms need to be preserved when a higher-order term is used in the model (for example, in a second-order polynomial regression model, the term *x* cannot be excluded

## My Approach to Variable Selection
My approach to variable selection is simple. I perform a EDA to understand the data, talk to the experts to understand the problem, and use criterion-based methods to select the variables for the model.

## Common Techniques or Approaches 
Here I briefly talk about some commonly used methods for model selection. Some are based on more sound theory than others. 

### Stepwise Procedures
The stepwise procedures in general have a lot of drawbacks but are widely applied. The following are some commonly used stepwise techniques:  
+ Backward Elimination: This is the simplest method where we apply ANOVA analysis to the model with all variables. We then drop the variables with p-value greater than the assumed type 1 error rate (alpha). We repeat the process till a desirable model is achieved
+  Forward Selection: This is an extension to backward elimination where we start with an initial model with no explanatory variables and check the p-values. We then add new variables and check the model efficacy
+  Stepwise Regression: This is a combination of backward elimination and forward selection

### Criterion-based Methods
The criterion-based methods are much preferred in general. Some common methods are:  
+  Akaike Information Criterion (AIC)  
+  Bayes Information Criterion (BIC)
+  Adjusted R^2

## Stepwise vs Criterion Methods 
Stepwise methods in general have more weaknesses. Here are some of them (paraphrased):  
+ The R^2 values are biased high
+  F Statistics do not have the claimed distribution
+  Standard errors and confidence intervals are too small
+  Collinearity is an issue

In addition, the stepwise methods use a restricted search approach for model selection. On the other hand, criterion-based models typically involve a wider search. The criterion-based models also penalize for the number of explanatory variables used in the model, achieving the simplest model. **I prefer using criterion-based methods** in general for variable selection in my models.  

