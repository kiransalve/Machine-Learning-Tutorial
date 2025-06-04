We have x data point on (x, y) axis.

![11](https://github.com/user-attachments/assets/5208ec29-947c-46bc-bc50-1b6a73faccc3)

Actually we can say point X is vector which have two component

One is on x direction and other is in y direction

so we have to project this X vector to another vector

(X ko dusare line pe girana hai)

the another vector is also has direction and (x, y) component

we have required direction of this vector

Suppose that another line is u vector

![12](https://github.com/user-attachments/assets/8ca25343-b1ac-472d-b08d-124b58aaf3a9)

and we have project X vector to u vector like this 

![13](https://github.com/user-attachments/assets/1e81e077-0262-402e-9ba6-940f97391e76)

the projection is (intersecting dot) and represented by

![14](https://github.com/user-attachments/assets/d6379fc8-e228-475e-b6e5-6ad5d5f5d7f6)

but in our case u is unit vector, so magnitude of u is 1

![15](https://github.com/user-attachments/assets/b51666cf-461b-4ec3-ba0e-30b06021d313)

u.x is u Transpose x

if we dot product of (x, y) of u and X

![16](https://github.com/user-attachments/assets/bca57f53-1086-43af-b7a2-9c3fe2996d07)

we get scalar - length

so for every data points we get one scaler - length

but we only choose u vector that has maximum variance

to get this for all we have formula 

![17](https://github.com/user-attachments/assets/54112986-b07f-4e0b-b9d5-bb33389d6887)

and we want maximum variance 

![18](https://github.com/user-attachments/assets/d2a884fd-fda6-42b1-adf6-a377e4b23af1)

there are many unit vectors but we want the vector that gives maximum variance

pca finds maximum value for this formula mathematically

now this become Optimization problem

to solve this problem we required high level of maths, so we ommit it and directly jump to solution.

before that we need to understand two mathamatical concept - 


# Covariance and Eigan Value

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


