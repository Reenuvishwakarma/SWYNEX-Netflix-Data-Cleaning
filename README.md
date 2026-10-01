# SWYNEX - Netflix Data Cleaning & Preparation

This project was completed as part of the **SWYNEX Internship – Data Cleaning & Preparation Task**. The objective of this project was to clean and prepare a real-world Netflix Movies and TV Shows dataset using **Python and Pandas**. The dataset was first inspected to identify data quality issues such as missing values, incorrect data types, duplicate records, and mixed data formats. Missing values in the `director`, `cast`, `country`, and `rating` columns were handled by replacing them with `Unknown` while preserving the original records. The `date_added` column was converted from an object/string format into a proper datetime format, while the 10 records with unavailable dates were retained as `NaT` instead of creating artificial values. The `duration` column contained different formats for Movies and TV Shows, such as minutes and seasons, so two new columns, `duration_minutes` and `seasons`, were created to make the information structured and easier to analyze. Duplicate records were checked using Pandas and no duplicate rows were found. Categorical columns such as `type`, `rating`, `country`, and `listed_in` were also inspected for obvious inconsistencies, and no major inconsistencies were identified. After cleaning and transformation, the dataset contained **7,787 rows and 14 columns**, with the original row count preserved. The cleaned dataset is now ready for further analysis, visualization, and dashboard development.

## Objectives

- Identify and understand data quality issues.
- Handle missing values appropriately.
- Convert columns to suitable data types.
- Transform inconsistent or mixed data formats.
- Check and validate duplicate records.
- Validate categorical values.
- Prepare a clean dataset for further analysis.

## Data Cleaning Performed

- Replaced missing `director` values with `Unknown`.
- Replaced missing `cast` values with `Unknown`.
- Replaced missing `country` values with `Unknown`.
- Replaced missing `rating` values with `Unknown`.
- Converted `date_added` from object to datetime.
- Retained unavailable dates as `NaT`.
- Extracted movie duration into `duration_minutes`.
- Extracted TV show seasons into `seasons`.
- Checked duplicate rows.
- Validated categorical columns.
- Preserved the original dataset without unnecessarily deleting records.

## Dataset Information

The dataset contains information about Netflix Movies and TV Shows, including title, type, director, cast, country, date added, release year, rating, duration, genre/category, and description.

**Original Dataset:** 7,787 rows and 12 columns  
**Cleaned Dataset:** 7,787 rows and 14 columns

## Technologies Used

- Python
- Pandas
- NumPy
- Jupyter Notebook
- Git
- GitHub

## Project Structure

```text
SWYNEX-Netflix-Data-Cleaning/
│
├── data/
│   ├── netflix_titles_unclean_dataset.csv
│   └── netflix_titles_Cleaned_dataset.csv
│
├── notebook/
│   └── Netflix_data_cleaning.ipynb
│
└── README.md
