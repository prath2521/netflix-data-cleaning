# Netflix Data Cleaning

## 🔍 Objective:
To clean and prepare the Netflix Titles dataset by handling missing values, removing duplicates, standardizing text formats, renaming columns, and fixing data types.

## 🛠 Tools Used:
- Python (Pandas)
- Jupyter Notebook

## 📄 Dataset:
- Source: [Kaggle Netflix Titles Dataset](https://www.kaggle.com/shivamb/netflix-shows)
- File: `netflix_titles_nov_2019.csv`

## ✅ Cleaning Steps:
1. **Missing Values**:  
   - Dropped all rows with missing values using `.dropna()`.

2. **Duplicate Records**:  
   - Removed duplicate rows using `.drop_duplicates()`.

3. **Standardized Text Fields**:  
   - Converted `type`, `country`, and `rating` columns to lowercase.

4. **Formatted Dates**:  
   - Converted `date_added` to `dd-mm-yyyy` using `pd.to_datetime()`.

5. **Renamed Columns**:  
   - Changed column headers to lowercase with underscores using `.str.lower().str.replace()`.

6. **Fixed Data Types**:  
   - Ensured `show_id` is string.
   - Converted `date_added` to datetime.

## 📁 Files Included:
- `netflix_titles_nov_2019.csv` – Raw dataset
- `cleaned_netflix_titles.csv` – Final cleaned dataset
- `netflix_cleaning.ipynb` – Notebook with all processing steps
