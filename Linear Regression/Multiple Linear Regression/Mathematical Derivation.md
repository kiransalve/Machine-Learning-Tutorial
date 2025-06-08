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
          n
y = Bo +  ∑ Bixi
         i=1

this will give us that our predicted value is how much depend upon the input columns

like is iq matters in package, if iq value is low then salary goes low or not?
if we have m columns and n students
matrix - 
   
|ŷ1|    |Bo   B1x11  B2x12  ...  Bmx1m |
|ŷ2|    |Bo   B1x21  B2x22  ...  Bmx2m |
|..|  = |...                           |
|..|    |...                           |
|ŷn|    |Bo   B1xn1  B2xn2  ...  Bmxnm |

|ŷ1|    |1 x11  x12  ...  x1m |  | Bo |
|ŷ2|    |1 x21  x22  ...  x2m |  | B1 |
|. |  = |. ...                |  | B2 |
|. |    |. ...                |  | .. |
|ŷn|    |1 xn1  xn2  ...  xnm |  | Bm |

By Matrix rule 
A B = AB

means first row of first matrix into whole second matrix 
and then so on

we can say 

ŷ = XB

Now we have y_train in data sets

    | y1 |
    | y2 |
Y = | .. |
    | .. |
    | yn |
          

now we have error matrix

e = y - ŷ

  | y1 |   | ŷ1 |
  | y2 |   | ŷ2 |
= | .. | - | .. |
  | .. |   | .. |
  | yn |   | ŷn |

  | y1 - ŷ1 |
  | y2 - ŷ2 |
= |    ..   |
  |    ..   |
  | yn - ŷn |


for single linear regression,
    n
E = Σ yi - ŷi
   i=1

we have to prove,

E = eTe

(T means transpose and B means Beta)

=[(y - ŷ)T (y - ŷ)

=(yT - ŷT)(y - ŷ)

=[yT - (xB)T) (y - xB)

=yTy - yTxB - (xB)Ty + (xB)T xB ....(1)

Detour

yTxB = (xB)Ty ....to prove

suppose 
y = A and xB = B

ATB = BTA

we know (AB)T = BTAT and (AT)T = A

(ATB)T = BTA

so we have to prove

ATB = (ATB)T

suppose ATB = C

C = CT

we need to prove 

(yTxB)T = yTxB

take the shape of (yTxB)

((1 X n) (n X (m + 1)) ((m + 1) X 1)

1 X (m + 1) (m + 1) X 1 

1 X 1

it is matrix like [ 7 ]

and [ 7 ]T is [ 7 ]

so proved

put this value in equetion (1)


=yTy - 2 yTxB + (xB)T xB

=yTy - 2 yTxB + xTBTxB

to get minimum value, we differentiate,

dE/dB = d/dB(yTy - 2 yTxB + xTBTxB)

= 0 - 2 yTx + d/dB(BTXTXB) = 0

= - 2 yTx + 2 xTxBT = 0

2 yTx = 2 xTxBT 

2 cancelled out

BT = yTx(xTx)-1 (inverse)

transpose both side

(BT)T = [ yTx (xTx)-1 ]T


B =  ((xTx)-1)T (yTx)T

B = ((xTx)-1)T xT


