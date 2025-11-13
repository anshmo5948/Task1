# 🧹 Data Cleaning Process (Excel)

This dataset initially had formatting issues and required several cleaning steps before analysis.  
The following transformations were performed **entirely in Excel**:

---

## 📌 1. Fixing Columns Using Text to Columns

The raw dataset had all values merged into a single column because Excel did not detect the tab delimiter.

**Steps performed:**
- Selected the entire column.
- Navigated to **Data → Text to Columns**.
- Chose **Delimited → Next**.
- Selected **Tab** as the delimiter.
- Clicked **Finish**.

This restored the dataset into properly separated columns.

---

## 📌 2. Handling Missing Values

- Checked for missing entries in all columns.
- Found missing values in the **Income** column.
- Replaced blank or undefined income values with **"N/A"** for consistency.

---

## 📌 3. Removing Duplicate Entries

- Selected all columns.
- Used **Data → Remove Duplicates**.
- No duplicate rows were detected after checking all fields.

---

## 📌 4. Standardizing Text Values

To ensure uniform formatting across categorical fields:

- Used **Find & Replace** to standardize text values in columns such as `Marital_Status`.
- Standardized values included:
  - **Single → single**
  - **Married → married**
  - **Together → together**

This ensures consistency for analysis and modeling.

---

## 📌 5. Formatting Date Columns

- Selected the `Dt_Customer` column.
- Applied **Format Cells → Date**.
- Set the format to **Short Date (dd-mm-yyyy)** to ensure uniform date formatting.

---

## 📌 6. Renaming Column Headers

To make column names consistent and analysis-friendly:

- Used **Find & Replace** to convert column names to lowercase and underscore format.
- Example updates:
  - `Year_Birth` ➝ `year_birth`
 

This standardization improves readability and compatibility with programming workflows.

---

✨ The dataset is now fully cleaned, structured, and ready for analysis.
