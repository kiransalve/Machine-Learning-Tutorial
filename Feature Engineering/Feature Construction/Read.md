Feature construction means creating new features 
from your existing data to improve the predictive power of your model.

Why?
Because raw data sometimes lacks meaningful representation for a model to learn well.

How?
By combining, transforming, or extracting information from existing features.


| Invoice\_ID | Invoice\_Date       | Customer\_Info          | Product\_Details       | Quantity | Price\_per\_Unit |
| ----------- | ------------------- | ----------------------- | ---------------------- | -------- | ---------------- |
| 1001        | 2025-06-01 15:45:23 | John Doe, New York, USA | A123-Red-Shirt-Large   | 3        | 499              |
| 1002        | 2025-06-02 11:10:10 | Jane Smith, Boston, USA | B234-Blue-Jeans-Medium | 2        | 799              |



1. Feature Splitting

Split Invoice_Date into multiple features:

Invoice_Date = 2025-06-01 15:45:23

Split into:

Invoice_Day = 1

Invoice_Month = 6

Invoice_Year = 2025

Invoice_Hour = 15


Split Customer_Info into:

Customer_Name = John Doe

Customer_City = New York

Customer_Country = USA


Split Product_Details into:

Product_Code = A123

Color = Red

Category = Shirt

Size = Large


2. Feature Construction

Create Total_Price = Quantity * Price_per_Unit:

For Invoice_ID 1001: 3 * 499 = 1497

Create Is_Peak_Hour based on Invoice_Hour:

If Invoice_Hour between 9 and 18, then Is_Peak_Hour = 1, else 0.

Create Customer_Location by combining City and Country:

Customer_Location = "New York, USA"


Why do this?

Splitting helps the model to understand each piece of info separately (e.g., Size might affect sales differently than Color).

Constructing new features like Total_Price or Is_Peak_Hour adds meaningful signals that can improve predictions or insights.

