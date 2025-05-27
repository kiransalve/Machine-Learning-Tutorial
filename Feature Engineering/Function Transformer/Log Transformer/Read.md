We take log of every value

When to Use :

not usefull for -ve value

if you have right skewed data it is better transform

It make very big value in common scale (equidistant)

![5aa77370-e302-4e19-b400-93292f472b62_3720x3184](https://github.com/user-attachments/assets/0030d356-724c-492c-88ea-4972ab7e2398)

Example 

![1_Bxf2uFMkfqLuWTZtrdlcGg](https://github.com/user-attachments/assets/bf0bf187-5b83-4482-942d-f9eba89e6762)



What is a Log Transformation?

A log transformation replaces a feature x with log(x) (commonly log(x + 1) to handle zero values).

For natural log: log(x) or np.log(x)

For base-10: np.log10(x)

For base-2: np.log2(x)

For zero or negative values: use log1p(x) → which computes log(x + 1)


When to Use Log Transformation?

When the feature is highly skewed (positively skewed).

When there's heteroscedasticity (variance changes with the mean).

When your model is assuming normality (like in Linear Regression).

When outliers dominate the learning process.


