(::----------Covariance----------::)

Covariance measures how two variables change together, indicating whether they move in the same or opposite directions

We cant find how much spread of data by looking of there mean value

In below case the mean is same but spread of data is different

![19](https://github.com/user-attachments/assets/2757a293-c2ef-4197-923f-7a26b059bef1)

to solve this problem we have variance

but variance have one issue, it only talk about spread of data for one axis

![20](https://github.com/user-attachments/assets/7c6f8b25-1b6b-465a-846a-487529b8dc11)

but if we have x and y axis then for x axis the variance is different and for y axis it is different

we cant get relation between x and y

variance may be similar for below type of data

![21](https://github.com/user-attachments/assets/2e69adda-45e9-4dee-b56b-95ddda506037)

we need what is relation between x and y

Covariance is calculated by taking the average of the product of the deviations of each variable from their respective means.

🤝 Simple Intuition:

If both variables increase together, covariance is positive.

If one increases while the other decreases, covariance is negative.

If the variables are independent, covariance is zero or near zero.

📊 Real-Life Analogy:

Imagine you're tracking:

Hours studied 📚

Exam score 📝

If students who study more generally score higher, then the covariance between hours studied and exam scores is positive.

![22](https://github.com/user-attachments/assets/007f7fe8-2f39-4f3a-8970-a5b5f98a4f83)

Read for Covariance Matrix -

https://github.com/kiransalve/Machine-Learning-Tutorial/blob/main/Feature%20Engineering/PCA/Covariance%20Matrix.md
