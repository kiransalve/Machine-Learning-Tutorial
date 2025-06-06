If we have input and output column in our data, it is Supervised Machine Learning Case

if the output column is numerical then it is solved by Linear Regression

also if we have only one input and output column then it called Simple Linear Regession.

If suppose we have CGPA and Package dataset, where the student's CGPA and thier actual package are given

Suppose one new student come and ask you that my CGPA is 7.4 what will be package my package?

In normal case what we do to answe his questin, we give avg of package like 3.5 LPA

But if we have past data where students of this much CGPA got this much package

then we can predict the package based on their CGPA using simple linear regression

what we do we simple plot graph of cgpa and package
To predict we need linear line that passes through all the data points
In real world their is no term called perfect linear data.

if it is then all can predict the stock prices, weather condition, even win dream 11 betting

and this is becasuse stochastic error, this error is not measurable, 

means some student get very less package in there data group, 

like from 5.0 to 5.5 data groups all other students got 3.5 LPA but one student gets 2.0 package,

this have multiple causes, like his interview not go well, now how can we measure Interview Bura Gaya?, kitna kharab gaya? cant quantify

In real world we have sort of linear data 

and we have find line which passes closely with all data points, called best fit line.

This line make least mistake than any other line

How to calculate best fit line?

To calculate best fit line we need slope and y-intercept

slop give how much our line is tild

y-intercept gives us distance from y-origin on y-axis

![Linear-Equations](https://github.com/user-attachments/assets/15d19e68-04ef-425f-8484-5c37f2cd6a2a)


this line tries to minimize the distance from data point and line

because if there is perfect line, that passes through all data point, and there is no distance between them

so the best fit line has some error with respective to each line (Har data-points se kam jyada distance hai)

we can get it from 

from sklearn.linear_model import LinearRegression

model = LinearRegression()

# m = slope (coefficient)
model.coef_

# b = intercept
model.intercept_

so in our case 

package = m X cgpa + b

m is like weightage

means how much package depends on cgpa

means for more the value of m the more the package, and vice versa

means if m (slope) is less then it tells that package less change with cgpa

means if m (slope) is large then it tells that package change hugely with cgpa


b is offset

kal ko agar m.x = 0 hua to kuch na kuch value chahiye, b is that value

suppose we have experice vs package column 

and our candidate have 0 year of experience then m.x will 0, to kya fresher ko salary nahi milegi?

milegi, kuch na kuch milegi, that kuch na kuch will be "b"...!

