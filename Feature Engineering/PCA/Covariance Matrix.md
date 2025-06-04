(::-------------Covariance Matrix-------------::)

The covariance matrix is a square matrix that shows the covariance between every pair of features (variables) in your dataset.

🔢 Example Dataset:

Let’s say you have 3 features:

![23](https://github.com/user-attachments/assets/1d5571e9-00ae-4749-86fd-1bad5f2051a2)

the formula is 

![image](https://github.com/user-attachments/assets/e5d73522-a6da-4858-be34-9780430fa967)

Diagonal: variances of individual features (e.g. Var(X₁), Var(X₂))

Off-diagonal: covariances between pairs (e.g. Cov(X₁, X₂))

📌 Properties:

The matrix is symmetric, i.e. Cov(X₁, X₂) = Cov(X₂, X₁)

Size is n X n where n = number of features

Positive values: variables increase together

Negative values: one increases while the other decreases

Zero: variables are independent


🧠 What is Eigen Decomposition of a Covariance Matrix?

