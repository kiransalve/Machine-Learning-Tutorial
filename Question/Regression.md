What is Linear Regression?

How does OLS work?

What assumptions does linear regression make?

What happens if assumptions are violated?

What is multicollinearity?

How to detect multicollinearity?

What is VIF?

What is overfitting?

What is underfitting?

What is bias–variance tradeoff?

Difference between Ridge and Lasso?

Why does L1 cause feature selection?

What is Elastic Net?

# What is R²?

R² (Coefficient of Determination) tells you:

How much variance in the dependent variable is explained by the model.

Formula logic:

Total variance in Y

Minus unexplained variance (residuals)

Divide by total variance

Interpretation:

R² = 0.80 → 80% of variation explained.

R² = 1 → Perfect fit.

R² = 0 → Model explains nothing

means how much you not studied,
if you got 60% marks then that means
you not studies 40%

Important:
It does NOT mean 80% accuracy.
It means 80% variance explained

# Why is R² misleading?

R² always increases when you add more features.

Even if those features are garbage

So:

Add random column → R² goes up.

Overfit model → R² goes up.

Add 100 useless variables → R² still goes up.

That means R² rewards complexity.

In real life:
High R² ≠ good model
It may just be memorizing noise.

# What is Adjusted R²?

Adjusted R² fixes that problem.

It penalizes unnecessary predictors.

Formula intuition:
It adjusts based on:

Number of features (p)

Number of observations (n)

If you add useless variable:

R² increases

Adjusted R² may decrease

Interview answer:

“Adjusted R² compensates for model complexity by penalizing additional predictors that do not improve model performance.”

# Difference between MAE and RMSE?

When to prefer RMSE?

When does linear regression fail?

How to handle non-linearity?
