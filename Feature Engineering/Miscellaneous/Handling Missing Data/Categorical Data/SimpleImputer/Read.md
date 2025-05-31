1. Imputation with Mode (Most Frequent Value)

Replace missing values with the most frequent category.

df['Category'] = df['Category'].fillna(df['Category'].mode()[0])

Good for: nominal (unordered) categories


2. Imputation with a New Category

Create a new category like "Missing" or "Unknown".

df['Category'] = df['Category'].fillna('Missing')

Good for: preserving information about missingness (especially useful in tree-based models)


3. Imputation with a Placeholder Like “Other”

If the missing value is rare, group it under "Other" or an infrequent label.

df['Category'] = df['Category'].fillna('Other')


 When to Avoid Dropping:
 
 Avoid dropping rows unless missing data is very minimal (<1%) or random.


 Always create a new column indicating missingness before imputation. It can be useful for modeling.

 df['Category_missing'] = df['Category'].isnull().astype(int)
