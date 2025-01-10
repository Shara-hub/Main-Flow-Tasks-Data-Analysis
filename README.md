# Data Analysis
 Learning Data Analysis  

import pandas as pd

# Load your dataset (replace 'your_dataset.csv' with your actual file)
df = pd.read_csv('your_dataset.csv')

# Data Exploration
# Get a summary of your dataset
print(df.info())
print(df.describe())

# Check for missing values
print(df.isnull().sum())

# Handle missing values
# Drop rows with missing values
df.dropna(inplace=True)

# Fill missing values with a specific value (e.g., 0)
df.fillna(0, inplace=True)

# Fill missing values with the mean of the column
df['column_name'].fillna(df['column_name'].mean(), inplace=True)

# Remove duplicate entries
df.drop_duplicates(inplace=True)
