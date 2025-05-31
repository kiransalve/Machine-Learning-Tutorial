1. Maximum Value Imputation

Replaces missing values with the max value of the column.

df['Feature'] = df['Feature'].fillna(df['Feature'].max())

2. Mean + 3×Standard Deviation (Right Tail)

Captures extreme upper-end values.

extreme_value = df['Feature'].mean() + 3 * df['Feature'].std()

df['Feature'] = df['Feature'].fillna(extreme_value)

We can also use mean + 2*std or mean + 1.5*IQR depending on how aggressive we want to be.

3. 99th or 95th Percentile Imputation

A robust way to capture the “end” of real data, especially if data is skewed.

percentile_value = df['Feature'].quantile(0.99)

df['Feature'] = df['Feature'].fillna(percentile_value)

