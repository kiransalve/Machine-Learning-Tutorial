
1. Square Transformation
   
What it does:

Applies 𝑥^2 to a feature.

Increases the effect of large values.

Makes left-skewed data more normal.

Use when:

Data is negatively skewed (left tail).

You want to emphasize large values.

Caution:

Can amplify outliers.

df['x_squared'] = df['x'] ** 2


2. Square Root Transformation
  
What it does:

Applies x**1/2 to a feature.

Reduces the impact of large values.

Mildly reduces right skewness.

Use when:

Data is slightly right-skewed.

You want to normalize spread without being too aggressive.

Caution:

Only works for non-negative values.

df['x_sqrt'] = np.sqrt(df['x'] + 1)

3. Reciprocal Transformation

What it does:

Applies 1/x
​
Strongly compresses large values.

Reduces right skewness significantly.


Use when:

Data is very right-skewed.

You want to flatten extreme values.


Caution:

Only works for non-zero values.

Avoid zero and negative values.

badi value choti ho jati hai,
choti value badi ho jati hai

df['x_reciprocal'] = 1 / (df['x'] + 1e-6)  # avoid division by zero



| Transformation | Use Case              | Effect on Skew        | Handles Zero  | Common Use        |
| -------------- | --------------------- | --------------------- | ------------- | ----------------- |
| `x ** 2`       | Left-skewed           | Increases skew        | ✅             | Feature expansion |
| `sqrt(x)`      | Slightly right-skewed | Mildly reduces skew   | ❌ (use +1)    | Variance control  |
| `1/x`          | Highly right-skewed   | Strongly reduces skew | ❌ (use +1e-6) | Compress outliers |


