Gradient Descent is an optimization algorithm used to minimize a cost or loss function in machine learning models.

It works by:

Calculating the gradient (slope) of the loss function with respect to the model’s parameters.

Updating the parameters in the opposite direction of the gradient to reduce the error.

Repeating this step iteratively until the algorithm converges to a minimum (ideally the global minimum).

![gd](https://github.com/user-attachments/assets/be4bc3fc-f478-4cff-b858-b159e3976568)

![gd1](https://github.com/user-attachments/assets/cf8c107d-4a78-4445-8140-f9d82098451a)

What is the role of the learning rate in gradient descent?

The learning rate (α) controls how big the steps are in each iteration. 

If it is,

Too low: The model learns very slowly, requiring many iterations to converge.

Too high: The model may oscillate or diverge, never reaching the minimum.

What do we mean by convergence in gradient descent? How do we know it has converged?

Convergence means the loss function stops decreasing significantly with each iteration. 

We check convergence by monitoring:

Change in cost function < small threshold (like 0.0001)

Gradient close to zero

Fixed number of iterations (if using early stopping)

What are the differences between Batch, Stochastic, and Mini-Batch Gradient Descent?

| Type                 | Description               | Pros                        | Cons                    |
| -------------------- | ------------------------- | --------------------------- | ----------------------- |
| **Batch**            | Uses entire dataset       | Stable, accurate            | Slow on large data      |
| **Stochastic (SGD)** | One data point per update | Fast, escapes local minima  | Noisy updates           |
| **Mini-Batch**       | Small subset per update   | Balance of speed & accuracy | Needs tuning batch size |


Can gradient descent get stuck in a local minimum? How do we handle that?

Yes, especially in non-convex functions. 

To handle it:

Use Stochastic Gradient Descent, which introduces noise and helps escape local minima.

Use momentum or advanced optimizers like Adam.

https://towardsdatascience.com/gradient-descent-clearly-explained-in-python-part-2-the-compelling-code-c21ee26fbc28/
