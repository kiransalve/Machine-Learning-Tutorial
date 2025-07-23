 What is interpolate() in pandas?

 interpolate() is used to fill missing values (NaNs) in a smart way by estimating the values based on existing data — often using linear interpolation.

 ```text

Simple Example:

import pandas as pd

data = {
    'Sales': [100, None, 300, None, 500]
}
df = pd.DataFrame(data)

print(df['Sales'].interpolate())

Output:

0    100.0
1    200.0   ← Estimated between 100 and 300
2    300.0
3    400.0   ← Estimated between 300 and 500
4    500.0
Name: Sales, dtype: float64

```

Intuition:

If one value is missing between two known values, interpolate() fills it by assuming a straight line between them.

Like joining the dots in a line chart.

```text

Common Methods:

df['col'].interpolate(method='linear')      # Default – line between points
df['col'].interpolate(method='time')        # For time series
df['col'].interpolate(method='polynomial', order=2)  # For curves

```


When to use:

Your data has numerical trends (like sales over time).

Missing values are inside the data, not at start or end (interpolate won't fill those unless you specify limit_direction).
