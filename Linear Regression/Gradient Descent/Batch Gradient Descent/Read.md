### Batch Gradient Descent

![batch-gradient-descent](https://github.com/user-attachments/assets/adbf8970-f4cf-44a2-af2d-3a6ae23d03c6)


Pure data ko dekhane ke bad slope caluclate karta hai

it is slow 

suitable for small data

sare row per ek update - Batch GD

rarely use

used for convex data, but dataset should not large

Introduction

Batch Gradient Descent is an optimization algorithm used in machine learning and deep learning to minimize a loss (or cost) function by updating model parameters iteratively. It is one of the most common forms of gradient descent, especially used in regression and neural networks.

🔍 Intuition:

Imagine you're trying to reach the lowest point in a valley (i.e., minimum cost). Batch gradient descent looks at the entire landscape before taking a step — it computes the direction (gradient) using all training examples before updating the parameters.

📘 Definition:

In Batch Gradient Descent, the model's parameters are updated by computing the gradient of the cost function using the entire training 
dataset.

🧠 Formula:

![gd2](https://github.com/user-attachments/assets/db9cf0b3-4bff-4564-909e-767d41bc0dec)



⚙️ Process:

Initialize weights (randomly or with zeros)

For each iteration:

Compute predictions on all data points

Compute the cost function (e.g., MSE)

Calculate the gradient (derivative of cost w.r.t. weights)

Update the weights

✅ Advantages:

Converges smoothly (less noise in gradient estimates)

Stable for convex problems like linear regression


❌ Disadvantages:

Slow for large datasets (because it processes the entire dataset for each step)

Not ideal for online or streaming data

✅ Use Cases:

Small to medium datasets

Convex optimization problems

Academic understanding of gradient descent

| Type                   | Data Used per Step | Speed    | Stability |
| ---------------------- | ------------------ | -------- | --------- |
| Batch Gradient Descent | All data           | Slow     | Stable    |
| Stochastic (SGD)       | 1 sample           | Fast     | Noisy     |
| Mini-batch             | Small batch        | Balanced | Good      |


