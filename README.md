# sales-data-analysis-using-python


This repository contains Python code for analyzing sales data using pandas, numpy, matplotlib, and seaborn. The dataset used is stored in a CSV file named "Sales Data.csv."

## Getting Started

Before running the code in this repository, ensure you have the required Python libraries installed. You can install these libraries using pip:

- numpy
- pandas
- matplotlib
- seaborn

You can install these libraries using pip:


pip install numpy pandas matplotlib seaborn


## Data Cleaning and Preparation

1. Import the necessary libraries and load the dataset:


import numpy as np
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns

df = pd.read_csv('Sales Data.csv', encoding='unicode_escape')


2. Data cleaning steps include dropping unrelated/blank columns, checking for null values, and dropping rows with null values:


df.drop(['Status', 'unnamed1'], axis=1, inplace=True)
df.dropna(inplace=True)


3. Data type conversion for the "Amount" column:


df['Amount'] = df['Amount'].astype('int')


## Data Analysis and Visualization

The code performs various data analysis and visualizations on the sales data, including:

- Count of Gender
- Total Amount vs Gender
- Count of Age Groups by Gender
- Total Amount vs Age Group
- Count of Marital Status
- Total Amount vs Marital Status by Gender
- Count of Occupation
- Total Amount vs Occupation
- Top 10 Product Categories by Sales Amount
- Top 10 Products by Orders

These analyses are visualized using bar charts and are available in the Jupyter Notebook provided in this repository.

## Conclusion

The code and visualizations in this repository provide insights into the sales data, helping to understand the distribution of sales across various categories. 
You can further customize and expand these analyses to gain more insights into the dataset.

