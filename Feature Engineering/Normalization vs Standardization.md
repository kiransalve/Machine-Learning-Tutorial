1. Defination

| Feature     | Normalization (Min-Max Scaling)                    | Standardization (Z-score Scaling)                   |
| ----------- | -------------------------------------------------- | --------------------------------------------------- |
| **Goal**    | Rescale data to a fixed range (usually 0 to 1)     | Center data around mean 0 with standard deviation 1 |
| **Formula** | $X_{norm} = \frac{X - X_{min}}{X_{max} - X_{min}}$ | $X_{std} = \frac{X - \mu}{\sigma}$                  |

2. Output Range
   
| Feature   | Normalization   | Standardization                      |
| --------- | --------------- | ------------------------------------ |
| **Range** | Usually \[0, 1] | Mean = 0, Std Dev = 1 (range varies) |

 3. Use Case

| Feature         | Normalization                                       | Standardization                                          |
| --------------- | --------------------------------------------------- | -------------------------------------------------------- |
| **When to Use** | When you know the data is bounded or in fixed range | When data is Gaussian (normal distribution) or unbounded |
| **Examples**    | Image pixel values (0–255), sensor readings         | Height, weight, salary, scores, z-scores, etc.           |
