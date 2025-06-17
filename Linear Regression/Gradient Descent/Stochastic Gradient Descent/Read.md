### Stochastic Gradient Descent

https://alanwiseblog.wordpress.com/2018/02/04/how-to-descend-a-hill/

![stochastic](https://github.com/user-attachments/assets/c6526b64-3411-45e1-be17-0b34dc397fdd)

Stochastic gradient descent can be thought of a drunk person walking down a hill.

Stochastic Gradient Descent (SGD) is a variation of gradient descent where the model parameters are updated 
using only one training example at a time rather than the entire dataset.

🔍 Intuition:

Imagine you're in a valley trying to reach the lowest point (minimum cost). 

Instead of analyzing the whole landscape (like batch GD), you just look at one stone (data point) and decide your next step. 

It's fast but a little noisy — it might bounce around, but it eventually gets to the bottom.

📘 Definition:

In SGD, you update your weights after each training sample, rather than after all samples.

🧠 Formula:

![gd4](https://github.com/user-attachments/assets/6f452fc3-537c-42a8-bced-185593e6ae59)


⚙️ Process:

Initialize parameters randomly

Shuffle the training data

For each epoch:

For each training example:

Make a prediction

Calculate error

Update the parameters using the gradient of that one example


✅ Advantages:

Fast and memory efficient (especially with large datasets)

Good for online learning (data streams in real-time)

Helps escape local minima due to its noisy updates

❌ Disadvantages:

Noisy convergence — the path is not smooth

May require more epochs to converge

Needs good learning rate tuning

🆚 Comparison Table:

| Feature                     | Batch GD          | SGD               |
| --------------------------- | ----------------- | ----------------- |
| Data per update             | All examples      | 1 example         |
| Update frequency            | Low               | High              |
| Convergence speed           | Slower (per step) | Faster (per step) |
| Convergence quality         | Smooth            | Noisy (bouncy)    |
| Suitable for large datasets | ❌                 | ✅                 |


✅ Use Cases:

Huge datasets (e.g., image classification, NLP)

Online learning systems (recommendations, ads)

Real-time model updates

