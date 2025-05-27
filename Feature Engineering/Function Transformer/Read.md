Some algorithms like linear regression, perform better on data that have normal distribution

many time data is not shows normal distribution

so we use below transformation 

1. Log transformation
2. Reciprocal
3. Power (sq/sqrt)

   also some mathematical
1. Box Cox
2. Yeo Hohnson
and custom transformation


How to find data is normal?

1. sns.distplot
2. pd.skew()
3. QQ plot

   
It's particularly helpful when your data has a long tail or exponential growth, which is common in real-world scenarios like:

Sales amount

Population

Income

Web traffic
