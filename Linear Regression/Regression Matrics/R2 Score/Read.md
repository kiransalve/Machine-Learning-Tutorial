 Formula for R² Score (Coefficient of Determination)

 ![r2](https://github.com/user-attachments/assets/192f071c-e060-40bd-9c38-5ee9ce66d81e)

![r21](https://github.com/user-attachments/assets/a7c98b3b-75ca-4d92-ad90-c5b5948c0155)

suppose we have only package column, and we want to predict the package.

we simply take average of all package and give that no. as predicted package

but now we have cgpa column

and we make linear regression model

so now we need to check how our LR model perform in compare to mean

as we devide LR model error with mean model error, that value represent that much our model doing mistakes

and subtracting by 1, gives % that that much % our model perform well than mean

also this score gives how much variance our model explain 

lets say r2 score is 0

r2 score will 0 if our lr/mean term will be 1

and lr/mean term will 1 when our lr model also same mistakes as mean line does.

so that means we have no use of cgpa

if r2 score 1

that means our lr/mean term will be 0 

and that means our lr term will 0

and that means our lr line not making any mistakes, goes through every data points

that means when our model performance is well, it moves towards 1 and 
that means when our model performance is worst it moves towards 0
