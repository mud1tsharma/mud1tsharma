These projects involve using provided APIs to obtain JSON or CSV data and then using Pandas to transform them into wide, timeseries data. In order to ensure data integrity, this also included things like:
- Detecting row and column names by parsing metadata or webpages
- Translating row and column names by parsing metadata or webpages
- Identifying time variables
- Splicing datasets to remove non-data rows

# 1. Federal Statistical Office, Germany
1. Obtain a list of ~2,000 datasets using the Requests module

2. For each dataset:
  - Determine if it is a valid timeseries
  - Create a corresponding DataFrame to store its metadata
  - Determine if it needs to be transposed
  - Create a dictionary to assist with German-English translations

3. Use the API and the parameters determined above to generate a wide, timeseries .CSV file



# 2. Monetary Authority of Singapore
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


