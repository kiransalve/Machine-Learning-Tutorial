Handling Missing Data

What is Complete Case Analysis (CCA)?

In CCA, you remove any row (observation) that has even one missing value in any of the columns (variables). 

Only fully complete rows are kept for analysis.

Example :

| ID | Age | Salary |
| -- | --- | ------ |
| 1  | 25  | 50,000 |
| 2  |     | 45,000 |
| 3  | 30  |        |
| 4  | 28  | 55,000 |

Using Complete Case Analysis, you would keep only row 1 and row 4, because rows 2 and 3 have missing values.


When to Use CCA:

1.When data is missing completely at random (MCAR) — meaning the missingness has no pattern and doesn't depend on any other variable.

2.When the number of missing rows is very small. (<5%)


Disadvantages:

Loss of data: You may throw away a large portion of your dataset.

Can lead to biased results if the missingness is not random.

Not suitable if missing data is common or systematic.

In production if missing data occurs, your model will not perform, because you didn't train it for handling missing data

