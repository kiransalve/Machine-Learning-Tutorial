Feature Scaling is a technique used to normalize the range of independent variables (features) in your dataset. 
It ensures that all features contribute equally to the model's performance.

Agar data ke numerical columns me ek column ki range bahot jyada aur dusare ki bahut kam hai to un dono columns ko ek range me lana.

E.g.
If we have Age and Salary columns in our dataset, 
age is limited to 60 or 90 max.
but salary is starting from 10,000 to 10,00,000 
when we plot graph, salary range will dominate
feature scaling make both in one scale - like  [0, 1] or [-1,1]

Two methods - 
Standardization and Normalization

Standardization - 
also known as Z-score Normalization

suppose we have Age column,
we transform each value by below formula
Xi' = Xi - mean / STD

mean - mu
STD - sigma

new age' columns have mean - 0 and STD - 1

![157194](https://github.com/user-attachments/assets/35b95fc2-d876-436c-b531-d49831e4b3a0)

pure data ko utha ke x aur y axis ke bich me rakhata hai

this is called "Mean Centering"

agar STD 1 se jyada hai, to ye data ko ander ki taraf dabata hai
agar STD 1 se kam hai, to ye data ko bahar ki taraf dhakelta hai
