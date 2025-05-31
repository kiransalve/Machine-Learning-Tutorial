We fill missing values from randomly selected values from training data

random values must be in data

we can apply it on numerical and categorical data

we do it in pandas, not in sklearn

Benifit

Easy to apply 

distribution will not change

Probability of random no. are more of most frequent data values

Best for linear model, not for decision tree


Disadvantage

Covarience will be disturbed

we need training data for random value to store in server, so memory heavy for large training data

X_train['Age_imputed'][X_train['Age_imputed'].isnull()] = X_train['Age'].dropna().sample(X_train['Age'].isnull().sum()).values




 
