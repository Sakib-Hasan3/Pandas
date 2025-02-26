
# Pandas 

Pandas is a powerful open-source Python library for data analysis and manipulation. Whether you're a beginner or looking to sharpen your data skills, this guide will help you get started with Pandas.  

---

## 📖 Free Pandas Learning Resources  

### 📝 Official Documentation & Guides  
- **[Pandas Official Documentation](https://pandas.pydata.org/docs/)** - Comprehensive documentation with examples and tutorials.  
- **[Pandas User Guide](https://pandas.pydata.org/pandas-docs/stable/user_guide/index.html)** - A structured guide covering essential Pandas functionalities.  

### 📚 Free Courses & Tutorials  
- **[DataCamp Pandas Tutorial](https://www.datacamp.com/tutorial/pandas-tutorial-dataframe-python)** - Beginner-friendly introduction to Pandas DataFrames and Series.  
- **[Kaggle Pandas Course](https://www.kaggle.com/learn/pandas)** - Hands-on Pandas exercises with real-world datasets.  
- **[Real Python Pandas Guide](https://realpython.com/pandas-python/)** - A step-by-step guide covering Pandas fundamentals.  
- **[FreeCodeCamp Pandas Tutorial (YouTube)](https://www.youtube.com/watch?v=vmEHCJofslg)** - A complete video tutorial for beginners.  

---

## 🔹 Pandas Basics  

### 📌 Installation  
You can install Pandas using pip:  
```bash
pip install pandas

📌 Importing Pandas
import pandas as pd

📌 Creating a DataFrame
data = {
    'Name': ['Alice', 'Bob', 'Charlie'],
    'Age': [25, 30, 35],
    'City': ['New York', 'Los Angeles', 'Chicago']
}

df = pd.DataFrame(data)
print(df)

Output:
     Name  Age         City
0   Alice   25    New York
1     Bob   30  Los Angeles
2  Charlie   35     Chicago

📌 Reading Data from a CSV File
df = pd.read_csv('data.csv')
print(df.head())  # Display the first 5 rows

📌 Basic Data Analysis
print(df.info())  # Summary of the DataFrame
print(df.describe())  # Statistical summary
print(df['Age'].mean())  # Calculate average age

📌 Selecting and Filtering Data
# Select a column
print(df['Name'])

# Filter rows where Age > 30
filtered_df = df[df['Age'] > 30]
print(filtered_df)

📌 Adding a New Column
df['Salary'] = [50000, 60000, 70000]
print(df)

📌 Sorting Data
df_sorted = df.sort_values(by='Age', ascending=False)
print(df_sorted)

📌 Grouping Data
grouped = df.groupby('City')['Age'].mean()
print(grouped)

📂 Example Pandas Projects
Awesome Pandas GitHub Repository - A curated list of useful Pandas resources and projects.
Pandas Data Analysis Examples - Practical exercises to improve your Pandas skills.
Kaggle Datasets - Find real-world datasets to practice Pandas.

If you have suggestions or improvements, feel free to submit a pull request! Let's learn and grow together.
