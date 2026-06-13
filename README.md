# Titanic Data Cleaning & Preprocessing

## Problem Statement

The objective of this project is to clean and preprocess the Titanic dataset to make it suitable for data analysis. The dataset contains missing values, unnecessary columns, and data type inconsistencies that need to be handled before analysis.

---

## Dataset Details

- **Dataset Name:** Titanic Dataset
- **Source:** Kaggle
- **File Used:** train.csv / titanic.csv
- **Number of Records:** 891
- **Number of Features:** 12

### Features in Dataset

- PassengerId
- Survived
- Pclass
- Name
- Sex
- Age
- SibSp
- Parch
- Ticket
- Fare
- Cabin
- Embarked

---

## Approach

### 1. Loading the Dataset
The dataset was loaded into a Pandas DataFrame using the `read_csv()` function.

### 2. Handling Missing Values

The dataset contained missing values in the following columns:

- Age
- Cabin
- Embarked

Actions performed:

- Missing values in **Age** were replaced using the median value.
- Missing values in **Embarked** were replaced using the mode value.
- The **Cabin** column was removed because it contained a large number of missing values.

### 3. Removing Duplicate Records

Duplicate rows were identified and removed using the `drop_duplicates()` function.

### 4. Data Type Conversion

The **Age** column was converted from float type to integer type for better consistency.

### 5. Renaming Columns

Column names were modified to improve readability.

Examples:

- PassengerId → Passenger_ID
- Pclass → Passenger_Class

### 6. Saving the Cleaned Dataset

The cleaned dataset was exported and saved as:

`cleaned_titanic.csv`

---

## Results

The following preprocessing operations were successfully completed:

✅ Missing values handled

✅ Duplicate records removed

✅ Data types converted

✅ Column names renamed

✅ Clean dataset generated successfully

---

## Technologies Used

- Python
- Pandas
- Google Colab

---

## Output Files

- Titanic_Data_Cleaning.ipynb
- cleaned_titanic.csv
- README.md

---

## Conclusion

The Titanic dataset was successfully cleaned and preprocessed. The resulting dataset is now ready for exploratory data analysis and further machine learning tasks.