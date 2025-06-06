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

If we have d distance from line for each point, (or we can say error made by line to cross data points)

like d1, d2, d3,....., dn

where n = total no. of data points

so total errors are
E = d1 + d2 + d3 + ..... + dn
the distance from line upper side will be positive (4,5,6,7)
and distance from line lower side be negetive (-2,-3,-4,-5)
so if we total them they will cancel each other and we cant get perfect total distance

so we will take square of each distances

why square, we can take |d1| modulus, to get total distance

Reason 1 - We want to panalize outlier, like if (5, 1) is distances, it becomes (25,1) 

Reason 2 - we will differentiate the above equestion and graph of mod is continueous but not differentiable at origin and graph of square is differentiable at any point

why square , why not power 4 or power 8
so if my work is done by square then why go beyond? (2 se kam chal raha hai to 4 kyo leu?)

E = d1^2 + d2^2 + d3^2 + .... + dn^2

We can write 

       n
E =    ∑ di^2
      i=1

E is error function
n = total no. data points
i = data points

So now we can say we want minimum value of this equetion

what is ditance, it is simply ditance between line and data point
and we this is respect to y value, like we have line at y^i and our original data point is at yi (in ml prediction denoted as hat (^))

so the distance is di = (yi - y^i) (actual packege - predicted packege)

rewrite equestion


       n
E =    ∑ (yi - y^i)^2
      i=1


now we want minimum value of above equestion

y^i = mxi + b

put value of y^i in E 



              n
E (m, b)  =   ∑  (yi - mxi - b)^2
             i=1


y and x is already in data, so you cant change them

you can only experiment values of m and b to find minimum value

m and b are line tuning knob, if we turn m or b our E will be change

suppose if b = 0

m is angle between x axis and y axis
it can be any degree 
suppose our all data points lies between 30 degree to 45 degree 

now if we turn our m (slope) from 0 degree to 15 degree our error (E) will get minimum
and at certain degree our error is minimum like at 36 degree
but after 36 degree error value become more and more 

so graph of E vs m is slightly parabolic

second case where m = 0
means we cant change angle but we can now change b (y values)

now suupose values y is from 0 to 7 LPA (Y is Package in LPA)
and if y - intercept is 1 then value of E (error) is more (more mistakes, more distance)
if we reduce y value and suppose at 0.07 error value is minimum, so we have line that closely pass through all data points
and we reduce further like at -0.5 error become more, our line makes more mistakes

so in both cases we get slightly paarbolic relation between E and (m, b)

so we have to find out the value of E where the m and b values are minimum

to find it we will do derivative of E w.r.t. m and b and then we make both equal to 0 

if E depends only on m then 
we simple do dE/dm = 0

but E depends on m as well as b, we have to use partial derivatives,

∂E/∂m = 0

and 

∂E/∂b = 0

we have to solve these both equestion so that we get minimum values of m and b
             n
∂E/∂b = ∂/∂b ∑ (yi - mxi - b)^2 = 0
            i=1


we have to do differentiation for each student, so we can place sigma outside,

∑ ∂/∂b (yi - mxi - b)^2 = 0

using chain rule,

∑  2(yi - mxi - b) * -1 = 0

because differentiation of yi and mxi will be 0 and b is -1

∑  - 2(yi - mxi - b) = 0

divide by -2

∑  (yi - mxi - b) = 0

we can write

∑yi - ∑mxi - ∑b = 0

if we divide all by n (total no. of students)

∑yi / n - ∑mxi / n - ∑b / n = 0

where 

∑yi / n is mean of y =  ȳ (average package of all students)

∑xi / n is mean of x = x̄ (average CGPA of all students)

and 

∑b / n is 

b + b + b + ... + b / n

so nb/n and nb/n = b (n is canceled out)


ȳ - mx̄ - b = 0

or we can write

b = ȳ - mx̄

this is equetion to find out the value of y intercept

to get value of m

we place value of b in below equetion


              n
E (m, b)  =   ∑  (yi - mxi - b)^2
             i=1



              n
E (m, b)  =   ∑  (yi - mxi - ȳ + mx̄)^2
             i=1

now we do partial differentiation of above,


∂E/∂m = ∑ ∂/∂m (yi - mxi - ȳ + mx̄)^2

using chain rule,

yi becomes 0
m becomes 1


∑ 2(yi - mxi - ȳ + mx̄) (- xi + x̄) = 0

∑ - 2(yi - mxi - ȳ + mx̄) (xi - x̄) = 0

divide by -2

∑ (yi - mxi - ȳ + mx̄) (xi - x̄) = 0

re-arrange,

∑ [(yi - ȳ) - m(xi + x̄)] (xi - x̄) = 0

∑ [(yi - ȳ)(xi + x̄) - m(xi + x̄)^2] = 0

∑ [(yi - ȳ)(xi + x̄) = ∑  m(xi + x̄)^2] 

so m becomes

    n                      n
m = ∑ [(yi - ȳ)(xi + x̄) /  ∑ (xi + x̄)^2
   i=1                    i=1


so this is value of m and b



















