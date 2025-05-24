Data has two types

Numerical and Categorical

Categorical data has two types

Nominal - States, Gender,Blood group, Department, City name, Product names
Ordinal - Education (School, Degree, PHD), Grade Class (1st Class, 2nd Class, Fail), Size (S, M, L)

If Y (output column) is categorical (Yes/No) type we use label encoding.

Ordinal Encoding is a technique used to convert ordinal categorical data into integers that reflect their natural order.

When to Use:

Use Ordinal Encoding when:

The categories have a clear ranking

You want to maintain the order in a machine learning model

Let’s take an ordinal feature:

Customer Satisfaction

| Customer Satisfaction | Ordinal Encoded |
| --------------------- | --------------- |
| Very Unsatisfied      | 1               |
| Unsatisfied           | 2               |
| Neutral               | 3               |
| Satisfied             | 4               |
| Very Satisfied        | 5               |


These numeric values now reflect the increasing level of satisfaction.


![ordinal](https://github.com/user-attachments/assets/69a17724-031c-45de-b4d2-1737c84b9711)

