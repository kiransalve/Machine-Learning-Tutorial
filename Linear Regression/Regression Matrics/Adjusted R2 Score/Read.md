Formula

![adjr2](https://github.com/user-attachments/assets/d3e94050-8095-4dd6-90cb-09d26b9b4463)

if we add irrelavent columns

then (1 - Rsqure) term increase little because adding new column will not able to explain more variation 
or we can say it can not decrease the mistake that our LR model making

and (n-1-k) will also decreases and it is decrease more compare to (1 - Rsquare) term

and so numerator is constant or less descrease and denominator decreases more 

so overall fraction will be increases, and subtracting by 1 the Adjusted R2 score will also decreases

if we add imporatant feature (column)

then (1 - Rsquare) term rapidly increases because adding new featire will explin more variation
or we can say it decreased mistakes our LR model do before adding that column

and now (n-1-k) also decreases but its decrease not more than (1 - Rsquare) term

so our numerator is more decreases than denominator 

and our fractions will decreases, and after subtracting by 1 the Adjusted R2 score will increases

If difference between R2 score and Adjusted R2 score is more then Adjusted R2 score is more reliable
