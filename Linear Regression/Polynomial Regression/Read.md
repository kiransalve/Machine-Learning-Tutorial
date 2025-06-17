## Polynomial Regression

https://www.tutorialspoint.com/machine_learning/machine_learning_polynomial_regression.htm

![linear_vs_polynomial_regression](https://github.com/user-attachments/assets/ed3cd499-a50f-4b09-9b48-3f8f9a52185b)

Polynomial Regression is a type of linear regression where the relationship between the independent variable x and 
the dependent variable y is modeled as an nth-degree polynomial. 

It is useful when your data shows non-linear patterns but you still want to use linear regression techniques.

![pr1](https://github.com/user-attachments/assets/14d4e6d4-b9a7-40fb-a178-4c645c9e2d01)


💡 Human Intuition:

Imagine you're drawing a curve that fits your data points. A straight line may not capture the bends or curves. 

Polynomial regression allows the model to bend to better fit the data by adding powers of x.

📌 When to Use:

Data shows a curved trend (U-shape or inverse U-shape).

Linearity assumption of simple linear regression fails.

You’ve plotted your residuals and see a pattern (non-random).

📈 Visualization Tip:

Always plot your predictions vs actual data. Polynomial regression can easily overfit if the degree is too high.

🚨 Important Interview Tips:

It’s still considered linear regression because coefficients are linear.

Polynomial regression increases the model complexity.

Always scale your data before polynomial transformation if you're using regularization (e.g., Ridge, Lasso).

https://www.tutorialspoint.com/machine_learning/machine_learning_polynomial_regression.htm
