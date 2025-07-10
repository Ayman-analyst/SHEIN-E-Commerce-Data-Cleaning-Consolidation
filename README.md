# 🛍️ SHEIN E-Commerce Data Cleaning & Consolidation

This project involves the cleaning, standardization, and merging of multiple SHEIN product datasets across various categories. The goal is to unify and preprocess the data for further analysis or modeling (e.g., price prediction, ranking analysis, etc.).

---

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

---

## 🧰 Technologies Used

- Google Colab  
- Python  
- Pandas  
- Seaborn  
- Matplotlib  

---

## 🗂️ Project Workflow

### 1️⃣ Dataset Loading
- Connected Google Colab with the Kaggle API.
- Downloaded and unzipped the SHEIN dataset.
- Loaded all 10 category-specific CSV files into separate Pandas DataFrames.

### 2️⃣ Initial Inspection
- Inspected column names and shapes.
- Identified and removed duplicate rows across all files.

### 3️⃣ Standardization & Cleaning
- Unified column names across all DataFrames:
  - `goods-title-link--jump` → `Product Title`
  - `selling_proposition` → `Selling Proposition`
  - `rank-title` → `Rank Title`
  - `rank-sub` → `Rank Subcategory`
  - `price`, `discount`, `color-count` standardized accordingly.
- Cleaned numerical values by:
  - Removing `$`, `%`, `k`, `+`, and text like “sold recently”.
  - Handling missing or null values in `Price`, `Discount`, `Color Count`, and `Selling Proposition`.
  - Converted string values into float or integer types.
- Created a new column `Selling Proposition Numeric` representing actual numeric values of sold units.
- Dropped unnecessary or HTML-based columns like `goods-title-link`.

### 4️⃣ Final Data Preparation
- Merged all cleaned DataFrames into one unified dataset (`main_df`).
- Ensured correct data types and no remaining missing values in key columns.

---

## 🧹 Cleaned & Final Columns

After transformation, the final dataset includes:
- `Product Title`
- `Price`
- `Discount`
- `Color Count`
- `Selling Proposition`
- `Selling Proposition Numeric` (converted to int)
- `Rank Title`
- `Rank Subcategory`

---

## 🧑‍💻 Author
- Ayman Mahmoud
- 📧 ayman.anaylst@gmail.com
- 📍 Giza, Egypt
- 🔗 LinkedIn Profile (https://www.linkedin.com/in/ayman-mahmoud-8b2287235/));
