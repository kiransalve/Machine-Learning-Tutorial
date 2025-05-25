What is a ColumnTransformer?

In Machine Learning, different types of columns (like numerical and categorical) 
often require different preprocessing steps.

The ColumnTransformer in scikit-learn allows you to apply different 
transformations to different columns in a single step.

Why Use It?

Numerical columns → need scaling

Categorical columns → need encoding

It keeps everything organized and clean, especially when building pipelines

Example - 

| Age | City   | Salary |
| --- | ------ | ------ |
| 25  | Mumbai | 50000  |
| 30  | Pune   | 60000  |
| 28  | Nashik | 55000  |


You want to use this data as input to your model.

But before that, you must prepare the data — because:

Age and Salary are numerical → need to be scaled

City is categorical → needs to be encoded

If you try to feed this directly into a machine learning model, it will throw an error or give bad results

So here we use ColumnTransformer

![column transformer](https://github.com/user-attachments/assets/8d3165d5-9b14-4b71-9652-1c320e96f25f)
