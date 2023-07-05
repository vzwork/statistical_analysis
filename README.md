# Project Overview

- Working with data from cell service provider
- Comparing two plans and identifying advantages of each

# Learning Points

- Practical experience of setting Null Hypothesis
- Practical experience testing the Null Hypothesis

# Statistical Analysis

Working with data starts from data preprocessing.

There are 2 main types of data and 2 subtypes:
- Qualitative Data (categorical)
  - Nominal
  - Ordinal - ranking option (education level - "BS", "MS", "PhD)
- Quantitative Data (numerical)
  - Discrete - integers
  - Continuous - floats

Depending on data type we use different preprocessing techniques:
- Qualitative Data
  - Use pandas.value_counts(<Series>) to examine the data
- Quantitative Data
  - Use <Series>.hist() to examine the distribution of data
  - Use numpy.var(<Series>) to find dispersion or varience (easier calculation)
  - Use numpy.std(<Series>) to find standard deviation or numpy.sqrt(numpy.var(<Series>))
  - Three-Sigma 65-95-99.7 rule helps us find outliers

Stratified random sampling - helps get a more general overview of the data.

Hypothesis Test
- Null hypothesis is working against the change
- If we calculate P-Value to be < (0.10, 0.05, 0.01), there has to be significant difference
- Then we can reject the null hypothesis

Calculating P-Value
- Independent Sample Test - scipy.stats.ttest_ind().p_value
- Paired Sample Test - scipy.stats.ttest_rel().p_value
- One Sample Test - scipy.stats.ttest_1samp().p_value

