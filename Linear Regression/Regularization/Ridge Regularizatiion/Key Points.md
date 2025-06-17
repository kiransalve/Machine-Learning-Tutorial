1. How the coefficients get affected?

λ value is lie between 0 to infinity

if λ value is 0 then it is linear regression

if we increase λ, all coefficient shrink towards zero but not become zero


2. Higher value are impacted more

if more value then decrease with more speed

i.e. higher values are impacted more than lower values


3. Bias Variance Trade off

if we increase λ, Bias is decreases (overfitting), variance increases

if we decrease λ, Bias is increased (underfiting) and variance decreases 

![ML--Bias-Vs-Variance-(1)](https://github.com/user-attachments/assets/b1b4bb00-8d7a-4b4a-ae87-fee59789f067)


4. Impact of loss function

As λ increases, the model emphasizes simpler, smaller-weight solutions even if it means accepting a bit more error.

This helps control overfitting and improves generalization.


5. Why called ridge?
   
![rigde](https://github.com/user-attachments/assets/fcd3e74b-e24b-4b15-9c6a-33957dba4272)

It's called Ridge Regression because the regularization constraint forms a ridge-like shape on the loss surface. 

Instead of freely optimizing the loss, the solution is restricted to lie on this curved ridge, where coefficients are balanced and shrinked — helping prevent overfitting.
