Outlier - Sharma ji ka beta, pure class ke pass hone ke lale pade hue hai, aur ise 99% mil ke bhi ro raha hota hai

Suppose in group we discuss our salary, some has 20,000, some has 30,000 and some has 40-50,000, 
but if elon musk comes in our group then our average salary will be in crores becuase he is outlier and skew the data.

Defination

An outlier is a data point that is significantly different from other observations in a dataset.


Weight based algorithm impacted by outlier

Tree based algorithm not impacted by outlier because they cut your data on certain condition

How to Treate?

1.Treaming - cut the outlier

2.Capping - Outlier always at end of distribution, will limit on certain threshold

3.Treat as missing outlier

4.Descritization/Binning


How to Find?

1.Normal Distribution

If data is outside of mean + 3*Std then it is outlier

2.Skewed Distribution

Box plot - if data is more than Q3 + 1.5IQR and less than Q1 - 1.5IQR

3.Other Distribution

99%tile or 2.5%tile 

Techniques

Z score

IQR

Percentile

Winserization

