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
  - Use pd.value_counts(<Series>) to examine the data
- Quantitative Data
  - Use <Series>.hist() to examine the distribution of data
  - Use numpy.var(<Series>) to find dispersion (easier calculation)
  - Use numpy.std(<Series>) to find standard deviation or numpy.sqrt(numpy.var(<Series>))
  - Three-Sigma 65-95-99.7 rule helps us find outliers


