# Creating-Pandas-Basic-DataFrame-Python
Pandas DataFrame Project 📊🐍

Welcome to my Pandas DataFrame Project! In this project, I'm exploring various fundamental operations on Pandas DataFrames — a powerful data structure for data analysis and manipulation in Python.

🔎 What I have Learned

In this project, I have learned and implemented the following essential Pandas operations:

Creating Pandas DataFrames from various Python collections.
Exploring DataFrame properties and retrieving information.
Selecting specific columns from the DataFrame.
Adding new columns to a DataFrame.
Renaming DataFrame columns.
Generating descriptive statistics on the columns.
### 📁 Project Overview

This project will guide you through how to work with Pandas to manage, manipulate, and explore tabular data. Here's what you can expect:

1. Creating Pandas DataFrames:
I start by showing how to create a DataFrame from different Python collections such as lists, dictionaries, and NumPy arrays. These are foundational steps to begin any data analysis project.

2. Learning About DataFrame Properties:
Next, we learn how to inspect the DataFrame’s properties and metadata. This includes:

Data types of each column (dtypes)
Dimensions of the DataFrame (number of rows and columns)
Quick info about the DataFrame structure (info())
Displaying the first few rows (head())
3. Selecting a Single Column:
I demonstrate how to select a single column from the DataFrame, allowing us to analyze specific data from a large dataset.

4. Adding New Columns:
In this step, we add new columns to the DataFrame. These could be based on existing columns or new data you want to include. We'll also look at adding columns conditionally.

5. Renaming Columns:
Renaming columns is a common operation when cleaning up data. We explore how to rename columns in a DataFrame to make them more descriptive or standardized.

6. Descriptive Statistics:
Finally, we perform some basic descriptive statistics on the DataFrame columns, including:

Mean, median, and mode
Minimum and maximum values
Standard deviation and variance This helps to summarize the data and understand its distribution and central tendencies.

### 📂 Files in This Repository

Pandasdataframes_01(1).ipynb And Pandasdataframes_01.py(Both files are same): The Python script that contains all the code for creating, manipulating, and analyzing the Pandas DataFrames.

### 🛠 Technologies Used

Colab Python (with Pandas library)
Jupyter Notebooks (optional, for interactive exploration)

### 📋 Example Code Snippets

Here’s a quick overview of some of the key operations used in the project:

Creating a DataFrame from a Dictionary
import pandas as pd

### Creating a dataframe from a list of dictionaries
basket = [
    {"item": "mango", "quantity": 4, "price": 2.99},
    {"item": "bread", "quantity": 2, "price": 3.25},
    {"item": "juice", "quantity": 1, "price": 5.90},
    {"item": "orange", "quantity": 3, "price": 2.99},
    {"item": "lime", "quantity": 3, "price": 0.3},
]
basket

df = pd.DataFrame(basket)
print(df)
### Creating a dataframe from a dictionary of lists
basket = {
    "item": ["mango", "bread", "juice", "orange", "lime"],
    "quantity": [4, 2, 1, 3, 3],
    "price": [2.99, 3.25, 5.90, 2.99, 0.30]
}
basket
pd.DataFrame(basket)

### Creating a dataframe from a list of lists
example = [
    [1, 2, 3],
    [4, 5, 6],
    [7, 8, 9]
]

column_names = ["variable_a", "variable_b", "variable_c"]
row_names = ["observation_1", "observation_2", "observation_3"]

pd.DataFrame(example, columns=column_names, index=row_names)
### Creating an empty dataframe
df = pd.DataFrame()

### Adding columns to a dataframe
### Any list-like data type can become a column
df["item"] = pd.Series(["Mango", "Bread", "Juice", "Orange", "Lime"]) #pandas series
df["quantity"] = [2, 2, 1, 3, 3] # list
df["price"] = (2.99, 3.25, 5.90, 2.99, 0.30) # tuple
df

### .shape returns rows, columns
df.shape

### len returns number of rows
len(df)
### size returns rows * columns
df.size
### 5 * 3 = 15

💡 What’s Next?

I will expand this project by working with more complex datasets and performing additional data analysis tasks.
I’ll explore data cleaning, missing values, and data visualization with libraries like Matplotlib and Seaborn.
