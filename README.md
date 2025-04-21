# 📊 Netflix Movies and TV Shows — Data Cleaning (Task 1)

## 🧠 About the Project

This project is part of a **Data Analyst Internship Task** focused on cleaning and preprocessing a real-world dataset.

The original dataset contains information about movies and TV shows listed on Netflix, including:
- Title
- Director
- Cast
- Country
- Date Added
- Release Year
- Rating
- Duration
- Genre
- Description

The primary goal of this task was to **identify and fix common data quality issues** like:
- Missing values
- Duplicate records
- Inconsistent formatting
- Irregular data types.

---

## 🧹 Cleaning Steps Performed

| Step                           | Action Taken                                               |
|--------------------------------|------------------------------------------------------------|
| **1. Missing Values**          | Filled missing values in `director` and `country` with `'Unknown'`. Converted `date_added` to datetime and handled invalid dates. |
| **2. Duplicate Records**       | Detected and removed duplicate rows to ensure unique data. |
| **3. Text Standardization**     | Cleaned `country` and `type` columns — removed extra spaces and converted text to Title Case. |
| **4. Column Name Cleaning**     | Renamed all column headers to lowercase with underscores for consistency (e.g., `Show ID → show_id`). |
| **5. Data Type Correction**     | Converted `date_added` to `datetime` format for accurate date-based analysis. |

---
# ALL THE DATA BEFORE AND AFTER CLEANING:

Missing Values:
show_id            0
type               0
title              0
director        2634
cast             825
country          831
date_added        10
release_year       0
rating             4
duration           3
listed_in          0
description        0
dtype: int64

Missing after conversion:
show_id           0
type              0
title             0
director          0
cast            825
country           0
date_added       98
release_year      0
rating            4
duration          3
listed_in         0
description       0
dtype: int64

Duplicate Rows: 0

Updated Columns:
 Index(['show_id', 'type', 'title', 'director', 'cast', 'country', 'date_added','release_year', 'rating', 'duration', 'listed_in', 'description'],
      dtype='object')

Data Types:
show_id                 object
type                    object
title                   object
director                object
cast                    object
country                 object
date_added      datetime64[ns]
release_year             int64
rating                  object
duration                object
listed_in               object
description             object
dtype: object


## 💾 Files Included

| File Name                      | Description                        |
|--------------------------------|------------------------------------|
| `netflix_titles.csv`           | Original raw dataset from Kaggle.  |
| `cleaned_netflix_titles.csv`   | Cleaned and processed dataset ready for analysis. |
| `Task1_Netflix_DataCleaning.ipynb` | Jupyter Notebook containing the full code and cleaning process. |
| `README.md`                    | This file — project summary and documentation. |

---

## ⚡ Tools Used

- **Python** — for scripting and data manipulation.
- **Pandas** — for handling tabular data.
- **Jupyter Notebook** — for exploratory analysis and step-by-step code.
- **Git / GitHub** — for version control and collaboration.

---

## 📚 Dataset Source

The original dataset is publicly available on Kaggle:  
[Netflix Movies and TV Shows Dataset](https://www.kaggle.com/datasets/shivamb/netflix-shows)

---

## 💡 Key Learning Outcomes

By completing this task, I learned:
- How to detect and handle missing values using `pandas.isnull()` and `fillna()`.
- How to identify and remove duplicate rows using `drop_duplicates()`.
- How to standardize text data and correct inconsistent entries.
- How to fix column names to make datasets clean and analysis-ready.
- How to prepare a dataset for downstream tasks like visualization and modeling.

---

## 🚀 How to Run the Code

1. Download the dataset `netflix_titles.csv`.
2. Open the `Task1_Netflix_DataCleaning.ipynb` notebook in Jupyter.
3. Run all the cells step by step.
4. The final cleaned file will be saved as `cleaned_netflix_titles.csv`.

---

## ✅ Submission Info

This project was completed for:  
**Data Analyst Internship — Task 1: Data Cleaning and Preprocessing**


---

## 💪 Author

- **KOUSTAV DUTTA**
- [https://www.linkedin.com/in/koustav-dutta-65a812208](Linkedin) (optional)
- GitHub: [Koustav-yogi](https://github.com/Koustav-yogi)

---
