# Name: Umesh Dhakal
# Course: MSCS634
# Professor: Dr. Satish Penmatsa
# February 28, 2026
# Lab 4- Regression Analysis with Regularization Techniques

## Purpose of the Lab
The purpose of this lab is to understand how different regression models work on real data. In this lab, I used the Diabetes dataset from scikit-learn to predict disease progression using health measurement features. I implemented and compared Simple Linear Regression, Multiple Linear Regression, Polynomial Regression, Ridge Regression, and Lasso Regression. The goal was to see how model performance changes when we use more features, add polynomial complexity, and apply regularization to reduce overfitting.

## Key Insights and Observations
From my results, using only one feature (bmi) in Simple Linear Regression gave a basic starting model, but it was not very accurate compared to the other models. Multiple Linear Regression performed much better because it used all the features, so it had more information to make predictions.

Polynomial Regression showed that increasing the degree does not always improve performance. Lower degrees did not give a big improvement, and a high degree (like degree 9) clearly caused overfitting. I noticed this because the training score increased, but the test score became worse (even negative), which means the model was learning noise instead of the real pattern.

Ridge and Lasso regression helped improve results slightly compared to basic multiple regression. Ridge shrinks coefficients to make the model more stable, while Lasso can shrink some coefficients to zero, which works like feature selection. In my lab, Lasso performed the best overall with the lowest RMSE and the highest R² among the models I tested. I also saw that alpha value matters a lot: smaller alpha keeps the model closer to normal regression, and very large alpha can underfit and reduce performance.

## Challenges
One challenge for me was choosing good polynomial degrees and alpha values. I solved this by testing multiple degrees for polynomial regression and multiple alpha values for Ridge and Lasso, then selecting the best results based on RMSE and R².
