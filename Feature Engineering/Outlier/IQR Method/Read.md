The IQR (Interquartile Range) method is a robust and widely-used technique to detect and handle outliers, especially when the data is not normally distributed.

IQR Basics:

Q1 (25th percentile): Lower quartile

Q3 (75th percentile): Upper quartile

IQR = Q3 - Q1

Outlier Detection Rule:

A data point is an outlier if:

![iqr](https://github.com/user-attachments/assets/2fff2a03-a5d6-4587-8d01-0b19f123d68f)

This range defines the acceptable bounds.

When to Use IQR Method:

For non-normal or skewed distributions

When your dataset has extreme values and you don’t want them to affect the average

For robust statistical analysis

Handling Outliers:

Remove them from the dataset

Cap them at boundaries (Q1 - 1.5×IQR or Q3 + 1.5×IQR)

Treat separately (flag for special attention)

Use transformations before reapplying IQR

