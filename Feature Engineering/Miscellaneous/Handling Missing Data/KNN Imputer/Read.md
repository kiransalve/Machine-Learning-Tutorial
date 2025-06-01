KNN imputer based on - You are like your most closest neighour

How to find closest neighour - using euclidean distance

K means how many neighour you want to compare

KNN - K-Nearest Neighbors

K = Number of neighbors (like 3, 5, etc.)

Nearest = Closest rows (similar data)

Neighbors = Other rows in the dataset


| Height | Weight | Age | Blood Pressure |
| ------ | ------ | --- | -------------- |
| 160    | 55     | 25  | 120            |
| 165    | 60     | ?   | 115            |
| 170    | ?      | 30  | 130            |
| ?      | 58     | 28  | 125            |

Step 1
Find K nearest neighour (like 2,3,5 etc)

Step 2
Take mean of their values (like for weight 55 + 60 + 58 / 3)


Euclidean Distance Formaula -

![euclidean](https://github.com/user-attachments/assets/ae22e5d6-e83a-4253-ac40-14664cec8c2d)


What is Euclidean Distance?

It’s the "straight-line" distance between two points.

Example in 2D:

If point A = (1, 2) and point B = (4, 6), then:

Euclidean distance = √[(4−1)² + (6−2)²] = √[9 + 16] = √25 = 5

Problem with NaN

If one value is missing:

A = (1, NaN)

B = (4, 6)

→ Normal Euclidean can't calculate this!

 Solution: nan_euclidean distance

It:

Ignores the missing values (NaNs).

Calculates distance using only the available (non-NaN) values.

Divides by number of available features, so the distance is fair.

![Capture](https://github.com/user-attachments/assets/8fef309e-65dc-4200-8497-2d88bc110618)

![Capture1](https://github.com/user-attachments/assets/b0278f41-2dfb-4681-9d75-4289630ea7b4)

Advantage/Disadvantage

More Accurate

More no. of calculations

Need to provide training data to server in production

Speed slow and memory heavy

Ideal for small data sets

better for mean/median/mode


