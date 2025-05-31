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

In simple words:

Z = 0 → You are exactly average

Z = +1 → You are 1 step above average

Z = -2 → You are 2 steps below average


What is Standard Deviation?

Standard deviation tells us how spread out or how far away the numbers in a group are from the average

Think of it like this:

If your class test scores are all very close to each other (like 60, 62, 61, 59), the standard deviation is small because the scores don’t vary much.

But if the scores are very different (like 30, 70, 90, 40), the standard deviation is big because the scores are spread out a lot.

Small standard deviation means most numbers are close to the average.

Large standard deviation means the numbers are very spread out.

Standard deviation = How much the numbers “move away” from the average on average.

In short:

Standard deviation = 2 → Most data points are about 2 units away from the average.

It's a measure of spread: smaller value = less spread, larger value = more spread.



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
