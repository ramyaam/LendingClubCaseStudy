## Analysis Steps

### 1. Data Loading
- Loaded the dataset from the CSV file into a Pandas DataFrame.

### 2. Initial Data Exploration
- Displayed the first 5 rows and examined column data types.
- Generated summary statistics for numeric columns.

### 3. Column Cleanup
- Dropped columns that are identifiers, descriptive text, or have high missing values across rows.

### 4. Handling Mixed Data Types
- Identified columns with mixed data types and analyzed further.

### 5. Data Type Conversion
- Created `int_rate_numeric` and `empl_length_numeric` columns by standardizing data formats.

### 6. Outlier Detection and Removal
- Applied IQR method to identify and handle outliers in columns like `loan_amnt`, `annual_inc`, etc.

### 7. Default Analysis
- Investigated default rates by loan grade and employment length.

### 8. Data Quality Assessment
#### Numerical Columns:
- **loan_amnt (Loan Amount):**
  - Checked for unusually high or low values.
  - Ensured all values are positive.
- **funded_amnt (Funded Amount):**
  - Compared with `loan_amnt` to ensure logical consistency.
- **funded_amnt_inv (Funded Amount by Investors):**
  - Ensured it's less than or equal to `funded_amnt`.
- **term_in_months (Term in Months):**
  - Verified typical values (e.g., 36 or 60 months).
- **int_rate (Interest Rate):**
  - Checked for values within the expected range.
- **installment_per_month (Monthly Installment):**
  - Verified logical consistency with `loan_amnt`, `term_in_months`, and `int_rate`.
- **employment_tenure_of_borrower_years (Employment Tenure in Years):**
  - Checked for valid ranges and unexpected values.
- **principal_received_to_date, interest_received_to_date, late_fees_received_to_date, recoveries, collection_recovery_fee, last_pymnt_amnt:**
  - Verified logical consistency and expected values.

#### Categorical Columns:
- **grade and sub_grade:**
  - Ensured valid values (A to G and their sub-grades).
- **home_ownership:**
  - Checked for expected values (RENT, OWN, MORTGAGE).
- **last_pymnt_month, next_pymnt_d, last_credit_pull_d:**
  - Ensured proper date formats and validity of dates.

### 9. Data Visualization
- Plotted graphs to explore relationships and dependencies between various factors and loan status.

### 10. Dependency Analysis
- Explored relationships such as Loan Amount vs Annual Income and Interest Rate vs Loan Purpose, grouped by Loan Status.
