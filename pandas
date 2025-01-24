# **Pandas Cheat Sheet for Machine Learning 📊**

A quick reference guide for essential **pandas** operations, focusing on data preprocessing, exploration, and manipulation. Easily copy and paste the code snippets you need!

---

## **📥 Importing Pandas**
```python
import pandas as pd
```

---

## **📂 Loading Data**

### **Load CSV File**
```python
df = pd.read_csv('data.csv')
```

### **Load Excel File**
```python
df = pd.read_excel('data.xlsx')
```

### **Load JSON File**
```python
df = pd.read_json('data.json')
```

### **Create DataFrame from Dictionary**
```python
data = {'Name': ['Alice', 'Bob'], 'Age': [25, 30]}
df = pd.DataFrame(data)
```

---

## **🔍 Exploring Data**

### **View First/Last Rows**
```python
print(df.head())   # First 5 rows
print(df.tail())   # Last 5 rows
```

### **Basic Information**
```python
print(df.shape)        # (rows, columns)
print(df.dtypes)       # Data types of each column
print(df.columns)      # Column names
print(df.describe())   # Summary statistics
```

### **Check for Missing Values**
```python
print(df.isnull().sum())
```

### **Unique Values in a Column**
```python
print(df['column_name'].unique())
```

---

## **🛠 Handling Missing Values**

### **Drop Missing Values**
```python
df.dropna(inplace=True)
```

### **Fill Missing Values**
```python
df.fillna(value=0, inplace=True)
df['column_name'].fillna(df['column_name'].mean(), inplace=True)
```

### **Interpolate Missing Values**
```python
df.interpolate(method='linear', inplace=True)
```

---

## **🧩 Feature Engineering**

### **Create New Column Based on Condition**
```python
df['new_column'] = df['Age'].apply(lambda x: 'Adult' if x >= 18 else 'Minor')
```

### **One-Hot Encoding (Categorical to Numerical)**
```python
df = pd.get_dummies(df, columns=['Category'], drop_first=True)
```

### **Label Encoding**
```python
df['Category_encoded'] = df['Category'].astype('category').cat.codes
```

---

## **📊 Data Selection and Filtering**

### **Select Specific Columns**
```python
df_subset = df[['Name', 'Age']]
```

### **Filter Rows by Condition**
```python
df_filtered = df[df['Age'] > 25]
```

### **Select Rows by Index Position**
```python
df.iloc[0:5]  # First 5 rows
```

### **Select Rows by Label**
```python
df.loc[df['Name'] == 'Alice']
```

---

## **📈 Data Aggregation and Grouping**

### **Group By and Aggregate**
```python
df_grouped = df.groupby('Category')['Sales'].sum()
```

### **Multiple Aggregations**
```python
df_grouped = df.groupby('Category').agg({'Sales': 'sum', 'Profit': 'mean'})
```

---

## **🔄 Data Transformation**

### **Rename Columns**
```python
df.rename(columns={'old_name': 'new_name'}, inplace=True)
```

### **Convert Data Types**
```python
df['Age'] = df['Age'].astype(int)
```

### **Normalization (Min-Max Scaling)**
```python
df['normalized'] = (df['Age'] - df['Age'].min()) / (df['Age'].max() - df['Age'].min())
```

### **Standardization (Z-score Scaling)**
```python
df['standardized'] = (df['Age'] - df['Age'].mean()) / df['Age'].std()
```

---

## **🗑 Handling Duplicates**

### **Remove Duplicate Rows**
```python
df.drop_duplicates(inplace=True)
```

### **Remove Duplicates Based on a Column**
```python
df.drop_duplicates(subset=['column_name'], inplace=True)
```

---

## **🔗 Merging and Joining DataFrames**

### **Merge Two DataFrames**
```python
df_merged = pd.merge(df1, df2, on='common_column', how='inner')
```

### **Concatenate DataFrames**
```python
df_concat = pd.concat([df1, df2], axis=0)  # axis=1 for columns
```

---

## **💾 Exporting Data**

### **Save to CSV**
```python
df.to_csv('output.csv', index=False)
```

### **Save to Excel**
```python
df.to_excel('output.xlsx', index=False)
```

### **Save to JSON**
```python
df.to_json('output.json')
```

---

## **📚 Additional Resources**

- [Pandas Official Documentation](https://pandas.pydata.org/docs/)
- [Pandas Cheat Sheet (PDF)](https://pandas.pydata.org/Pandas_Cheat_Sheet.pdf)
- [Machine Learning with Pandas Tutorial](https://www.kaggle.com/learn/pandas)

---

Enjoy coding with **pandas**! 🚀 If you find this guide helpful, feel free to share. 😊
