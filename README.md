# 🚗 Cars Data Analysis Using Python

A data analytics project that explores and analyzes a car dataset using Python and Pandas. The project demonstrates essential data analysis operations such as data cleaning, missing value handling, filtering, transformation, and extracting insights from automotive data.

## 📌 Project Overview

Automobile datasets contain valuable information about vehicle specifications, fuel efficiency, weight, cylinders, origin, and manufacturers.

This project performs Exploratory Data Analysis (EDA) on car data to understand vehicle characteristics and practice real-world data manipulation techniques using Pandas.

---

## 🎯 Objectives

- Explore and understand the structure of a car dataset.
- Identify and handle missing values.
- Perform statistical analysis.
- Filter data based on specific conditions.
- Transform and modify dataset columns.
- Extract meaningful insights from automotive records.

---

## 🛠️ Technologies Used

- Python
- Pandas
- Jupyter Notebook

---

## 📂 Project Structure

```text
Cars_Data_Analytics/
│
├── Cars_Data_Analytics.ipynb
├── Cars_Data.csv
├── README.md
└── requirements.txt
```

---

## 📊 Analysis Performed

### Data Exploration

- Dataset preview using `head()`
- Dataset dimensions using `shape`
- Understanding column structure

### Data Cleaning

- Detecting missing values
- Counting null values in each column
- Replacing missing values using mean imputation

### Manufacturer Analysis

- Counting vehicles by manufacturer
- Frequency analysis using `value_counts()`

### Conditional Filtering

Examples include:

- Cars originating from Asia
- Cars originating from Europe
- Vehicles above specific weight limits
- Removing records based on conditions

### Data Transformation

- Updating fuel efficiency values
- Applying transformations using Lambda Functions
- Column-wise operations with Pandas

---

## 🔍 Key Questions Solved

### 1. Find Missing Values

```python
cars.isnull().sum()
```

### 2. Replace Missing Cylinder Values

```python
cars['Cylinders'].fillna(
    cars['Cylinders'].mean()
)
```

### 3. Count Vehicles by Manufacturer

```python
cars['Make'].value_counts()
```

### 4. Show Cars from Asia or Europe

```python
cars[
    (cars['Origin'] == 'Asia') |
    (cars['Origin'] == 'Europe')
]
```

### 5. Remove Vehicles Weighing More Than 4000

```python
cars[~(cars['Weight'] > 4000)]
```

### 6. Increase City MPG by 3

```python
cars['MPG_City'] = cars['MPG_City'].apply(
    lambda x: x + 3
)
```

---

## 📈 Skills Demonstrated

- Data Cleaning
- Exploratory Data Analysis (EDA)
- Missing Value Handling
- Data Filtering
- Data Transformation
- Statistical Analysis
- Pandas Operations
- Python Programming

---

## 🚀 Getting Started

### Clone Repository

```bash
git clone https://github.com/Jignash-GH/Cars_Data_Analytics.git
```

### Navigate to Project

```bash
cd Cars_Data_Analytics
```

### Install Dependencies

```bash
pip install pandas notebook
```

### Launch Notebook

```bash
jupyter notebook
```

Open:

```text
Cars_Data_Analytics.ipynb
```

---

## 📚 Learning Outcomes

Through this project, the following concepts were practiced:

- Working with real-world datasets
- Handling missing data
- Data filtering using logical conditions
- Applying transformations using functions
- Extracting business insights from data
- Efficient DataFrame manipulation

---

## 👨‍💻 Author

**Jignash**

GitHub:  
https://github.com/Jignash-GH

LinkedIn:  
(Add Your LinkedIn Profile)

---

## ⭐ About This Project

This project was developed to strengthen practical data analytics skills using Python and Pandas by solving common real-world data analysis problems on an automobile dataset.

If you found this project useful, consider giving it a ⭐.
