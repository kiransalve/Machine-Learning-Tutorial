Standardization is a feature scaling technique where we transform the data to have a mean of zero and a standard deviation of one. 

The formula is straightforward — we subtract the mean and divide by the standard deviation for each feature.

If the value is greater than mean then it is positive and if less than mean it is negetive

I typically apply standardization in pipelines where the algorithms are sensitive to the scale of data, 
like Logistic Regression, SVM, KNN, and Neural Networks. 

For instance, if I'm working on a classification model using logistic regression, and 
one feature like sales amounts is in lakhs while another like products quantity is a small integer, 
the model might disproportionately weigh the sales amount unless I standardize both.

In my last project, I was building a customer churn prediction model. 
After exploratory analysis, I noticed that features like customer age, average transaction value, 
and number of visits per month had very different scales. So, before feeding the data into 
a Random Forest and Logistic Regression model, I used StandardScaler from scikit-learn to standardize the numeric features. 

It helped improve the convergence of the model and gave better performance metrics, especially for logistic regression.
