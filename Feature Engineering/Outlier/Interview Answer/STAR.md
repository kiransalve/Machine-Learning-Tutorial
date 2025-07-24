An outlier is a value that is very different from the rest of the data.

# It is much higher or lower than most of the other numbers.

Suppose we have group of freinds and we have salary discussion, some have 40,000, some have 30,000, some have salary 35,000 and in 
our group Elon musk entered, so average of our salary is go much higher.

When i am doing EDA for our poultry division sales data, their are several outlier like when the bird flue is there sales drop significantly
and also in month of ramazan eid sales spikes, also we have one export order which is one time order it is much higher than our monthly sales

To find these outlier i used boxplot like 

sns.boxplot(x=df["Sales"])

What is a Box Plot?



