------------ 2 ------------

MSE - Mean Square Error (Loss function)

We use square instead of mod

![mse1](https://github.com/user-attachments/assets/f5a531e1-47c1-4699-8e11-b6573b4ab67f)

![mse2](https://github.com/user-attachments/assets/74e4df52-681b-4afc-aba3-ea5365fa56fb)

🧠 Intuition:

First, calculate how wrong the prediction

Then square that error so:

o Negative errors don’t cancel out positives

o Larger errors are penalized more

Finally, take the average over all data points

Advatage :

It is differentiable

Disadvatage :

If MAE - 1.2 , then we can say, our model do mistake by 1.2 LPA

but in case of MSE it is  not interpretable, it is sqaure of unit 

also it panalize outlier, not robust to outlier

