## Monetary Authority of Singapore (MAS)

1. Using Regular Expressions, and HTML content:
  - Obtain a list of lists to represent the ~50 datasets made available by MAS

2. Using the Requests module:
  - Obtain table metadata
  - Clean outdated or incompatible metadata
  - Identify the time variable (daily, monthly, quarterly, or yearly)

3. Using the Requests module:
  - Recursively use the provided API to obtain batches of each table
  - Append these together, and use the obtained metadata to contextualise each Pandas DataFrame

4. Save each of these ~50 timeseries as CSV files
