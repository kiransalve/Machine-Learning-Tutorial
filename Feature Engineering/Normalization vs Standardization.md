1. Defination

| Feature     | Normalization (Min-Max Scaling)                    | Standardization (Z-score Scaling)                   |
| ----------- | -------------------------------------------------- | --------------------------------------------------- |
| **Goal**    | Rescale data to a fixed range (usually 0 to 1)     | Center data around mean 0 with standard deviation 1 |
| **Formula** | $X_{norm} = \frac{X - X_{min}}{X_{max} - X_{min}}$ | $X_{std} = \frac{X - \mu}{\sigma}$                  |

2. Output Range
   
| Feature   | Normalization   | Standardization                      |
| --------- | --------------- | ------------------------------------ |
| **Range** | Usually \[0, 1] | Mean = 0, Std Dev = 1 (range varies) |
