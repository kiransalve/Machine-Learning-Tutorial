![pipeline](https://github.com/user-attachments/assets/aa535b52-a7c0-420c-a0e6-766908ef19e0)


An ML pipeline is a structured way to automate the machine learning process—from data cleaning to model training. 

I typically start by handling missing values, scaling numeric features, and encoding categorical ones using tools like ColumnTransformer. 

Then, we wrap these steps into a Pipeline along with the model—like a Random Forest or Logistic Regression. 

This ensures that every step runs in the correct order, reduces the chance of data leakage, and makes the workflow more reproducible and production-ready
