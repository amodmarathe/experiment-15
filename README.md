1. Data Binning (Categorization)
pd.cut(x, bins, labels): The primary tool used to segment and sort data values into discrete bins. It was used to create categories for:

Price: Segmented into 'Low', 'Medium', and 'High'.

Units Sold: Categorized as 'Low Sales', 'Medium Sales', or 'High Sales'.

Order Value: Grouped into 'Low', 'Medium', and 'High' orders.

Delivery Time: Classified as 'Fast', 'Average', or 'Slow'.
Distance: Defined as 'Short', 'Medium', or 'High' distances.

2. Data Formatting & Cleaning
df.dtypes: Used to inspect the data types of each column in the DataFrame.

astype(float): Converted integer columns (like Units_Sold) into floating-point numbers.

str.upper(): Standardized text data by converting product names and Order IDs to all uppercase letters.

round(decimals): Used to round numerical values (like Price) to a specific number of decimal places.

3. Data Organization & Analysis
sort_values(by, ascending, inplace): Used to arrange the dataset based on specific columns (e.g., sorting by Price in both ascending and descending order).

unique(): Identified and displayed the distinct category labels present in a binned column.
value_counts(): Provided a frequency count of how many entries fell into each created category (e.g., counting the number of 'High Orders').

Conclusion
By utilizing binning and formatting techniques, raw numerical data can be transformed into meaningful categorical insights and standardized formats, 
significantly improving the readability and analytical value of a dataset.
