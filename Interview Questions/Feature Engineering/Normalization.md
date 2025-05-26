Normalization is a technique used to scale numeric features to a fixed range, typically 0 to 1. 

The goal is to bring all the features onto the same scale, especially when the algorithm relies on distance calculations — 
like K-Nearest Neighbors, K-Means Clustering, or any model where the scale can bias the results.

The formula for normalization, also known as Min-Max scaling, is:
Xi - Xmin / Xmax - Xmin

I prefer normalization when the data does not follow a Gaussian (normal) distribution, 
or when I’m using bounded algorithms like Neural Networks with sigmoid activation, where inputs are expected to be in the 0 to 1 range.

For example, in one of my projects involving customer segmentation using K-Means, I had features like total purchase amount, 
number of transactions, and days since last visit. 
Since K-Means relies on Euclidean distance, I used MinMaxScaler to normalize these features — otherwise, the large purchase amounts would dominate the clustering behavior
