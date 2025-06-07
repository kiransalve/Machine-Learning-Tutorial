Regression metrics are used to evaluate the performance of a regression model — 
i.e., models that predict continuous numeric values (like price, temperature, salary, etc.). 

--------------------- 1 ---------------------

💡 What is MAE - Mean Absulute Error

It’s the average of the absolute differences between actual values and predicted values.

🧠 Human Intuition (Simple Example)

Imagine you're predicting the price of used bikes.

Let’s say these are the actual vs. predicted prices:

| Bike | Actual Price | Predicted Price | Error   | Absolute Error |
| ---- | ------------ | --------------- | ------- | -------------- |
| A    | ₹10,000      | ₹9,000          | -₹1,000 | ₹1,000         |
| B    | ₹15,000      | ₹16,000         | +₹1,000 | ₹1,000         |
| C    | ₹12,000      | ₹11,000         | -₹1,000 | ₹1,000         |


Now take the average of those absolute errors:

![mae1](https://github.com/user-attachments/assets/4230dddb-7ec6-4906-a646-24e695ee8993)

✅ So what does this ₹1000 mean?

On average, your predictions are ₹1000 away from the true price.

You don’t care if you were ₹1000 above or below — just how far you were.

Think of it like saying:

“My prediction is usually off by ₹1000.”

🧭 Why use Absolute Error?

Because sometimes:

A ₹-1000 error (under-predict) and ₹+1000 error (over-predict) can cancel each other out if we just summed the raw errors.

Taking absolute value avoids this and gives a true sense of how wrong we are.

💬 Real-Life Analogy:

Imagine you're telling your friend how much you'll be late to dinner.

Day 1: 10 minutes early

Day 2: 15 minutes late

Day 3: 5 minutes early

If you average raw error:

(−10+15−5)/3=0 minutes (looks perfect!)

But that's misleading — you're not always on time.

Now take absolute values:

(10+15+5)/3=10 minutes (more honest!)

This 10 minutes is your MAE — how far off you are on average, regardless of direction.

![mae2](https://github.com/user-attachments/assets/caa57d95-492a-46d2-b671-6bc6f186c509)

![mae3](https://github.com/user-attachments/assets/729de062-0ade-47b8-abe8-d22541af4f54)

Our job is to reduce this no.

Advantage 

The no. is exactly unit of y (like lpa, sales rs, minutes etc)

Robust to outlier less effect

Disadvantage

modulus function's graph is not differential at zero, it is biggest gap

when we use algorithm like gradient descent, it fails

This problem solved by MSE - Mean Square Error

