# Week 2: Working with DataFrames (Pandas Basics)

## 📚 Overview

This week you'll learn to work with structured data using Pandas, Python's most important library for data analysis. We'll focus on loading, exploring, and cleaning real datasets related to social issues.

## 🎯 Learning Objectives

By the end of this week, you will be able to:

- Load datasets from CSV files into Pandas DataFrames
- Explore dataset structure (rows, columns, data types)
- Perform basic data cleaning operations
- Calculate summary statistics and understand data distributions
- Handle missing values and rename columns appropriately
- Filter and sort data to answer specific questions

## 🎓 Session Structure (80 minutes)

### Lecture (40 minutes): Introduction to Structured Data

**Topics Covered:**
- What are DataFrames and why they matter for social impact analysis
- Loading data from CSV files using `pd.read_csv()`
- Exploring dataset structure: `.shape`, `.info()`, `.head()`, `.tail()`
- Understanding different data types: numbers, text, dates
- Basic indexing: selecting rows and columns

### Tutorial (40 minutes): Cleaning a Real Social Dataset

**Hands-on Activities:**
- Load a dataset about global education or health indicators
- Explore the data structure and identify issues
- Clean the dataset: drop missing values, rename columns
- Calculate basic statistics (mean, median, counts)
- Create simple data transformations

## 🏗️ Mini-Deliverable

**Assignment:** Create a notebook that summarizes key statistics of a real dataset related to social impact.

**Requirements:**
1. **Load a provided dataset** about education, health, or development
2. **Explore the data structure** using Pandas methods
3. **Clean the data** by handling missing values and renaming columns
4. **Calculate summary statistics** (mean, median, min, max, counts)
5. **Answer 3 specific questions** about the data using filtering/grouping
6. **Document your findings** with clear explanations

### Example Analysis Structure:
```python
import pandas as pd

# Load dataset
df = pd.read_csv('global_education_data.csv')

# Explore structure
print(f"Dataset shape: {df.shape}")
print(f"Columns: {df.columns.tolist()}")
print(df.info())

# Clean data
df = df.dropna(subset=['literacy_rate'])  # Remove missing literacy rates
df = df.rename(columns={'GDP_per_cap': 'gdp_per_capita'})  # Cleaner names

# Summary statistics
print(f"Average literacy rate: {df['literacy_rate'].mean():.1f}%")
print(f"Countries with data: {df['country'].nunique()}")

# Answer specific questions
high_literacy = df[df['literacy_rate'] > 95]
print(f"Countries with >95% literacy: {len(high_literacy)}")
```

## 📁 Files Structure

```
week2/
├── README.md
├── notebooks/
│   ├── lecture_pandas_intro.ipynb
│   ├── tutorial_data_cleaning.ipynb
│   └── assignment_dataset_summary.ipynb
├── data/
│   ├── global_education_indicators.csv
│   ├── world_health_data.csv
│   └── sustainable_development_goals.csv
├── examples/
│   └── sample_analysis.ipynb
└── resources/
    ├── pandas_cheatsheet.md
    └── common_data_issues.md
```

## 📖 Key Concepts Introduced

### Pandas Fundamentals
- **DataFrame**: 2D labeled data structure (like a spreadsheet)
- **Series**: 1D labeled array (single column)
- **Index**: Row labels for data identification
- **Columns**: Variable names in your dataset

### Essential Pandas Methods
```python
# Loading data
df = pd.read_csv('filename.csv')

# Exploring structure
df.shape          # (rows, columns)
df.info()         # Data types and missing values
df.head()         # First 5 rows
df.describe()     # Summary statistics

# Data cleaning
df.dropna()       # Remove missing values
df.fillna(0)      # Fill missing values
df.rename(columns={'old': 'new'})  # Rename columns

# Basic analysis
df['column'].mean()     # Average
df['column'].nunique()  # Count unique values
df.groupby('category').mean()  # Group analysis
```

### Data Cleaning Best Practices
- Always explore your data first
- Document what cleaning steps you take
- Keep track of how many rows you remove
- Use meaningful column names
- Check for duplicates and outliers

## 🎥 Video Resources

1. **Why DataFrames Matter for Social Impact** (10 min)
2. **Loading and Exploring Data with Pandas** (15 min)
3. **Data Cleaning Essentials** (20 min)
4. **Calculating Summary Statistics** (10 min)

## � Sample Datasets

This week you'll work with real datasets related to:

### Option 1: Global Education Data
- Literacy rates by country and year
- School enrollment statistics
- Educational spending per capita
- Gender gaps in education

### Option 2: World Health Indicators
- Life expectancy by country
- Infant mortality rates
- Healthcare spending
- Disease prevalence data

### Option 3: Sustainable Development Goals
- Progress towards UN SDG targets
- Poverty reduction indicators
- Environmental sustainability metrics
- Gender equality measures

## 🔗 Additional Resources

### Pandas Documentation
- [Pandas User Guide](https://pandas.pydata.org/docs/user_guide/)
- [10 Minutes to Pandas](https://pandas.pydata.org/docs/user_guide/10min.html)
- [Pandas Cheat Sheet](https://pandas.pydata.org/Pandas_Cheat_Sheet.pdf)

### Social Impact Data Sources
- [World Bank Open Data](https://data.worldbank.org/)
- [UN Data](http://data.un.org/)
- [Our World in Data](https://ourworldindata.org/)
- [Gapminder](https://www.gapminder.org/data/)

## ❓ Common Questions

**Q: The dataset has thousands of rows. Do I need to analyze all of them?**
A: No! Start with a subset using `.head(100)` or filter to specific countries/years you're interested in.

**Q: What if there are many missing values?**
A: First understand why data is missing. Sometimes missing data tells a story (e.g., countries not reporting certain indicators).

**Q: How do I know if my data cleaning is correct?**
A: Always check before and after: print the shape, look at samples, and verify your cleaning makes sense.

**Q: Can I use my own dataset?**
A: Yes! As long as it's related to social impact and has at least 100 rows with multiple columns.

## 🆘 Getting Help

- **Discussion Forum**: Ask about specific Pandas errors
- **Office Hours**: Tuesdays 6-7 PM
- **AI Assistants**: Great for explaining Pandas syntax
- **Peer Support**: Share datasets and cleaning strategies

## 📈 Assessment Criteria

Your dataset summary notebook will be evaluated on:
- **Data Loading**: Successfully imports and explores dataset
- **Cleaning Process**: Appropriate handling of missing data and column names
- **Summary Statistics**: Meaningful calculations with clear interpretation
- **Analysis Quality**: Answers to questions show understanding of the data
- **Documentation**: Clear explanations of what you found

---

**Next Week**: [Week 3: Data Visualization with Plotly](../week3/README.md)

**Previous Week**: [Week 1: Welcome & First Steps in Python for Data](../week1/README.md)
