The Percentile Method is simple and effective technique for outlier detection and removal, 
especially useful for non-normal or heavily skewed datasets.

What Is the Percentile Method?

This method defines outliers as values that fall below a certain lower percentile or above a certain upper percentile, commonly:

Lower Bound: 1st percentile (or 5th percentile)

Upper Bound: 99th percentile (or 95th percentile)

Steps to Use Percentile Method:

Choose your lower and upper percentile thresholds (e.g., 1% and 99%).

Calculate the actual cutoff values from your data using these percentiles.

Flag or remove data points that fall outside this range.

When to Use This Method:

When your data is not normally distributed

For large datasets where removing a few percent won't harm

In financial or sales data, where extreme highs or lows are not relevant for some types of analysis

Things to Keep in Mind:

You manually choose the cutoffs (e.g., 1%, 99%) — choose based on domain knowledge.

Better for business rules-based outlier handling than purely statistical approaches.

Don’t use this method blindly — visualize data (boxplots, histograms) before applying.
