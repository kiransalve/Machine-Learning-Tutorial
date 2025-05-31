Standardization - 

also known as Z-score Normalization

Why is it called Z-score normalization?

Because we change each number to a Z-score, which tells:

"How far is this number from the average?"

What is a Z-score?

A Z-score tells you how far a number is from the average, using standard units.

Think of it like this:

Imagine your class has an average test score of 60 marks, and most students scored between 50 and 70.

If you got 75, the Z-score tells:

"How far is 75 from the average score of 60?"

suppose we have Age column,
we transform each value by below formula


![stand](https://github.com/user-attachments/assets/8abb2119-f3db-42d0-9773-bff316723202)


mean - mu
STD - sigma

new age' columns have mean - 0 and STD - 1

![157194](https://github.com/user-attachments/assets/35b95fc2-d876-436c-b531-d49831e4b3a0)

pure data ko utha ke x aur y axis ke bich me rakhata hai

this is called "Mean Centering"

agar STD 1 se jyada hai, to ye data ko ander ki taraf dabata hai
agar STD 1 se kam hai, to ye data ko bahar ki taraf dhakelta hai
