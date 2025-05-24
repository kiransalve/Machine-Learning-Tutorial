What is One-Hot Encoding?

Many machine learning models cannot understand words or categories like “Red”, “Green”, “Blue”.

They understand only numbers.

But we can't just give "Red = 1", "Green = 2", "Blue = 3" — because that would wrongly suggest some order or ranking, which doesn’t exist here.

So we use One-Hot Encoding to solve this.


Example

Let’s say we have a column of colors:

| Color |
| ----- |
| Red   |
| Green |
| Blue  |


We convert this into new columns like:

| Color\_Red | Color\_Green | Color\_Blue |
| ---------- | ------------ | ----------- |
| 1          | 0            | 0           |
| 0          | 1            | 0           |
| 0          | 0            | 1           |


Each row has only one 1 and the rest are 0s — that’s why it's called “One-Hot”.

The term comes from digital electronics, where a “one-hot” signal means only one line is active (1) out of several.


What is the Dummy Variable Trap?

The dummy variable trap is a situation that occurs when you use one-hot encoding (or dummy variables)
and include all the categories, which leads to multicollinearity — a problem for some models like linear regression.

What is Multicollinearity?

Multicollinearity means that one column can be predicted from the others.
This makes it hard for the model to understand which variable is actually important, and it distorts the model’s coefficients.


![Multicollinearity](https://github.com/user-attachments/assets/cb5cdbd2-9020-480b-9186-d1aaf80b477a)


Example:

Let’s say you have a feature called Color with 3 categories: Red, Green, Blue.

After one-hot encoding:

![one hot enco](https://github.com/user-attachments/assets/22f930e2-4385-4790-9e0f-00b1b2feeedd)

Now here's the catch:

If you know Red and Green, you can always calculate Blue:

Blue = 1 - (Red + Green)

That means these columns are not independent — and this causes multicollinearity.

Solution: Drop One Column

To avoid the dummy variable trap, drop one of the columns. You’ll still have all the information.

