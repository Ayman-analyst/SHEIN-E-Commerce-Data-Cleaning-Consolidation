# 🛍️ SHEIN E-Commerce Data Cleaning & Consolidation

This project involves the cleaning, standardization, and merging of multiple SHEIN product datasets across various categories. The goal is to unify and preprocess the data for further analysis or modeling (e.g., price prediction, ranking analysis, etc.)

## 📦 Dataset

The data is sourced from Kaggle:
[E-Commerce Data - SHEIN](https://www.kaggle.com/datasets/oleksiimartusiuk/e-commerce-data-shein)

It consists of 10 separate CSV files, each representing a SHEIN product category, such as:
- Appliances
- Automotive
- Baby & Maternity
- Bags & Luggage
- Home & Kitchen
- Home Textile
- Kids
- Office & School Supplies
- Tools & Home Improvement
- Underwear & Sleepwear


## 🧰 Technologies Used

- Google Colab
- Python
- Pandas
- Seaborn & Matplotlib


## 🗂️ Project Workflow

### 1️⃣ Dataset Loading
- Connected Google Colab with Kaggle API.
- Downloaded and unzipped the SHEIN dataset.
- Read all 10 category-specific CSV files into individual DataFrames.

### 2️⃣ Initial Inspection
- Identified duplicate records and dropped them.
- Explored column structures and shapes across all files.

### 3️⃣ Standardization & Cleaning
- Unified column names across datasets for consistency.
- Removed unwanted characters (e.g., `$`, `%`, `k`) from numeric fields.
- Handled null values for key columns such as:
  - `Price`, `Discount`, `Color Count`
  - `Selling Proposition` (converted to numeric scale)
  - `Rank Title`, `Rank Subcategory`
- Converted columns to appropriate data types (float, int, string).

### 4️⃣ Final Data Preparation
- Dropped unnecessary columns (e.g., raw HTML links).
- Merged all cleaned DataFrames into one `main_df` containing all categories.
- Verified that the final dataset is free of nulls and correctly typed.

---

## 🔍 Sample Columns After Cleaning

- `Product Title`
- `Price`
- `Discount`
- `Selling Proposition` (e.g., number of units sold)
- `Rank Title`
- `Rank Subcategory`
- `Color Count`


 🧑‍💻 Author
- Ayman Mahmoud
- 📧 ayman.anaylst@gmail.com
- 📍 Giza, Egypt
- 🔗 LinkedIn Profile (https://www.linkedin.com/in/ayman-mahmoud-8b2287235/));
