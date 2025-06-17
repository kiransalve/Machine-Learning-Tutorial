### Mini-Batch Gradient Descent

![mini-batch](https://github.com/user-attachments/assets/0d86d83f-61b7-498f-a0ff-123d9033cbea)


Mini-Batch Gradient Descent combines the best of both Batch Gradient Descent and Stochastic Gradient Descent (SGD). 

Instead of using the entire dataset (like Batch GD) or just one sample at a time (like SGD), 

it uses a small group of rows (a mini-batch) to update the model parameters.


🔍 Intuition:

You're trying to walk down a valley. 

Instead of relying on the whole landscape or just one stone, you look at a small patch of land — more stable than SGD, 
but faster than batch GD.


📘 Definition:

In Mini-Batch GD, you split your dataset into batches of size k (e.g., 32, 64, 128), and for each batch:

Compute the gradient using only that mini-batch

Update the model parameters

![gd5](https://github.com/user-attachments/assets/6bae3e34-f82e-437d-8aea-3bd6dce764a6)


⚙️ Process:

Shuffle the dataset

Split it into mini-batches of size k

For each epoch:

For each mini-batch:

Compute predictions

Calculate loss

Update weights using gradients from that mini-batch

✅ Advantages:

Faster convergence than Batch GD

Less noisy than SGD

Takes advantage of matrix operations (optimized in libraries like TensorFlow, PyTorch)

Parallelizable

❌ Disadvantages:

Need to tune the batch size carefully

Not as stable as batch GD, and not as fast (per update) as SGD
