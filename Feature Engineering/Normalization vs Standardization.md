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

4. Algorithm Sensitivity
   
| Feature         | Affects which algorithms?                                                             |
| --------------- | ------------------------------------------------------------------------------------- |
| **Both** affect | Distance-based models like **KNN**, **SVM**, **Logistic Regression**, **Neural Nets** |

5. Example

Let’s say:

X = 70

Min = 50, Max = 100

Mean = 65, Std Dev = 10

| Method          | Calculation                              | Result |
| --------------- | ---------------------------------------- | ------ |
| Normalization   | $(70 - 50) / (100 - 50) = 20 / 50 = 0.4$ | 0.4    |
| Standardization | $(70 - 65) / 10 = 5 / 10 = 0.5$          | 0.5    |


Summary

| Feature              | Normalization    | Standardization             |
| -------------------- | ---------------- | --------------------------- |
| Range                | \[0, 1]          | Mean = 0, Std Dev = 1       |
| Affected by outliers | Yes              | Less sensitive              |
| Best for             | Bounded features | Gaussian/unbounded features |
| Formula              | Min-Max Scaling  | Z-Score                     |
