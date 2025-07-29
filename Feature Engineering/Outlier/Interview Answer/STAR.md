# What is Oulier?

An outlier is a value that is very different from the rest of the data.

It is much higher or lower than most of the other numbers.

Suppose we have group of freinds and we have salary discussion, some have 40,000, some have 30,000, some have salary 35,000 and in 
our group Elon musk entered, so average of our salary is go much higher.

When i am doing EDA for our poultry division sales data, their are several outlier like when the bird flue is there sales drop significantly
and also in month of ramazan eid sales spikes, also we have one export order which is one time order it is much higher than our monthly sales

To find these outlier i used boxplot like 

sns.boxplot(x=df["Sales"])

----> What is a Box Plot?

Box plot also known as Box-and-Whisker plot

Box Represent :

The rectangular box represents the interquartile range (IQR) — the middle 50% of the data.

The left edge of the box is the first quartile (Q1) (25th percentile).

The right edge of the box is the third quartile (Q3) (75th percentile).

A line inside the box shows the median (Q2).

Whiskers represent :

The lines extending from both sides of the box

They typically go from:

Q1 to the smallest value within the acceptable range (i.e., not considered an outlier).

Q3 to the largest value within the acceptable range.

Small Circles represents :

Points beyond the whiskers are considered outliers.

I also finds the oulier using statistical methods like IQR method and Z score method

---> What is IQR Method

IQR (Interquartile Range) is the range between the first quartile (Q1) and the third quartile (Q3).

To find it we subtract the 3rd Quartile by 1st Quartile

IQR = Q3 − Q1

---> How do you handle them?
There are three main methods to handle outlier

first is remove them if they are less than 5% of total counts

second is cap then (also called as winserize) if they are valid but we need to reduce the infulence of these

third is make new column for them if they are important like promotional sales

In our model we cap them at certain limit and make high qty binary feature like normal order and high qty order 

