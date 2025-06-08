---------------- Multiple Linear Regression -----------------

Multiple Linear Regression is a method used to predict a value based on two or more inputs (factors or features).

Multiple Linear Regression is extended version of Simple Linear Regression

Where in Simple Linear Regression we have one input and one output column, 
in Multiple Linear Regression we have more than one input coumns and one output column

like in Simple Linear Regression we have CGPA and Package 
in Multiple Linear Regression we could have CGPA, Gender, IQ, Package

In real world scenario, we get Multiple Linear Regression problems mostly

For Simple Linear Regression,
y = mx + b

For Multiple Linear Regression,

y = mx1 + mx2 + b

for Simple Linear Regression we drow a line to find best fit line that closely passes through all data points

in Multiple Linear Regression like for 2 input columns we have to drow a plan that cut all points closely

for every n input column we have n + 1 coefficient

so if you have 3 input columns then we drow hyper plan, (for infinite column it called hyper plan only)

For 2 input columns,
          
y = mx1 + mx2 + b, (we have to find minimum values of m and b)

we can write,

![ml1](https://github.com/user-attachments/assets/aab5d0fd-1541-41a2-8ff7-a46b6e758e9e)

![ml2](https://github.com/user-attachments/assets/d4dfa441-d6bd-4c2b-a639-6a7904bf02e2)


🧠 Human Intuition (with β)

Imagine:

"I want to predict your monthly expenses based on income (x₁), number of children (x₂), and location cost index (x₃)."

The equation becomes:

![ml3](https://github.com/user-attachments/assets/da63de02-167f-4c13-b045-1184c7c0f2b7)

![ml4](https://github.com/user-attachments/assets/7fa10fcc-c7a0-407c-9d49-731b967d0e73)

for 3 input columns,

y = Bo + B1x1 + B2x2 + B3x3 (we have to find value of Bo, B1, B2, B3)

for n input columns,

y = Bo + B1x1 + B2x2 + ... + Bnxn

Or we can write 

Multiple Linear Regression — Summation Form

![ml5](https://github.com/user-attachments/assets/48dbd5fa-580b-4626-ae09-387219ed86a5)

![ml6](https://github.com/user-attachments/assets/d705a22c-e401-48e8-b65b-543bf73832d1)

this will give us that our predicted value is how much depend upon the input columns

like iq ka kitna hath hai package badhane me , gender kitna matter karta hai package ke liye...

if beta 1 is greater than beta 2 then we can say cgpa is matter more than iq to predict package

