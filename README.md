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

### 8. Data Visualization
- Plotted graphs to explore relationships:
  - Loan Status vs Loan Amount
  - Employment Tenure vs Loan Status
  - Home Ownership vs Loan Status
  - Annual Income vs Loan Status
  - Interest Rate vs Loan Status
  - Purpose vs Loan Status
  - Term in months vs Loan Status
  - Grade vs Loan Status

### 9. Dependency Analysis
- Explored dependencies between factors like Loan Amount vs Annual Income and Loan Status.
- Analyzed Interest Rate vs Loan Purpose grouped by Loan Status.
