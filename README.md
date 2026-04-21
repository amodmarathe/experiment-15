## Aim 

To understand and implement different data normalization techniques and data type conversion methods using Python libraries such as Pandas, NumPy, and preprocessing tools from Scikit-learn.

# Theory 

## 1. Data Normalization

Data normalization is a data preprocessing technique used to scale numerical values into a specific range so that all features contribute equally during analysis or machine learning.

Normalization is especially useful when working with machine learning algorithms that are sensitive to feature scaling.
Why Normalization is Important
1)Removes bias caused by different feature scales
2)Improves performance of machine learning models
3)Makes data easier to compare
4)Helps gradient-based algorithms converge faster

Types of Normalization Used

## 1. Min-Max Normalization

Min-Max normalization scales the values between 0 and 1.

Formula
X
norm
​

=
X
max
	​
−X
min	​

X−X
min
	​
	​

Example

Used for normalizing the Price column in the dataset.

## 2. Z-Score Normalization (Standardization)

Z-score normalization transforms data based on mean and standard deviation.

Formula
Z=
σ
X−μ	​


Where:
μ = mean
σ = standard deviation
Advantages
Centers data around 0
Useful for normally distributed data
3. Decimal Scaling

In decimal scaling, values are scaled by moving the decimal point.

Formula
X
scaled	​

=
10
j
X
	​

Where j is chosen so the maximum absolute value becomes less than 1.

Example:
Price ÷ 100000

# Data Encoding Techniques 

Machine learning models require numerical data, so categorical data must be converted.


## 1. Label Encoding
Each category is assigned a unique integer value.

Example:

Male → 1
Female → 0

Implemented using Scikit-learn LabelEncoder.

Advantages
Simple
Requires less memory
Limitation

May introduce false ordinal relationships.

## 2. One-Hot Encoding
Creates separate binary columns for each category.
Example for Payment Method:

UPI	Credit Card	Debit Card	COD
1	0	0	0

Implemented using Pandas get_dummies().

# 3. Dummy Encoding
Similar to One-Hot Encoding but drops one column to avoid multicollinearity.
Example:
If there are 4 categories → only 3 columns are created.


# Applications 

Data normalization and encoding are widely used in:
1)Machine Learning
2)Data Mining
3)Data Analytics
4)Artificial Intelligence
5)Recommendation Systems

# Conclusion 
In this experiment, various data preprocessing techniques were implemented. Numerical data was normalized using Min-Max, Z-score, and Decimal Scaling methods, 
while categorical data was converted into numerical format using Label Encoding, One-Hot Encoding, and Dummy Encoding. These preprocessing steps are essential for improving the performance and accuracy of machine learning models.
