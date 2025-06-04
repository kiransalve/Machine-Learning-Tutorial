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

Covariance and Eigan Value



