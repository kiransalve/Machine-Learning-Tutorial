Also called L2

Overfitting - your model perform expepsionally great on training data 

In tearms of Linear regression the value of m (slope) will be higher in overfitting case

Ridge Regression is a type of linear regression that includes L2 regularization, which adds a penalty equal to the square of the magnitude of coefficients to the loss function.

This penalty term prevents the model from assigning excessively large weights to features, which helps reduce overfitting. It works well when all features are useful but may be correlated, and we want to keep all of them in the model without eliminating any.

The hyperparameter λ (alpha) controls the strength of regularization — higher λ leads to more shrinkage.

![ridge](https://github.com/user-attachments/assets/1385a78d-f987-4afd-948b-0473461a0873)

![ridge_rigression_test_theory__1](https://github.com/user-attachments/assets/b5d7e108-d78f-4d03-83d8-545604f0010d)

