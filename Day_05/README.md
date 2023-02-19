# Regression Loss Functions

## Topics covered in today's module
* Mean Squared Error
* Mean Absolute Error
* Mean Squared Logarithm Error

## Main takeaways from doing today's assignment
MSE penalizes larger errors more than smaller errors due to the squared term. MAE, on the other hand, treats all errors equally and only looks at the average magnitude of errors. MSE is often used in models where larger errors have more negative impacts on the model's performance, while MAE is useful when we need a more robust metric that is less sensitive to outliers.

MSLE, as compared to MSE and MAE, measures the ratio between the actual and predicted values rather than the difference between them. This makes it particularly useful for regression tasks where we care more about the relative difference between the actual and predicted values rather than the absolute difference. MSLE can also handle negative numbers, unlike MSE.

## Challenging, interesting, or exciting aspects of today's assignment
It was exciting to use other loss function

## Additional resources used 
https://www.analyticsvidhya.com/blog/2021/05/guide-for-loss-function-in-tensorflow/
