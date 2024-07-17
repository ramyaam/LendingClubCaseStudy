# LendingClubCaseStudy
<br>
<br>
## Steps taken for the analysis
<br><br>
 1. Loaded the data into a datafram from the csv file
 <br>
 2.Printed the top 5 rows from the dataframe and the column data types to understand the data<br>
 Also get the summary statistics
 <br>
 3.Identified and dropped columns which are row identifiers or description text or columns which have  Null or NAN or same value for all rows 
 <br>
 4. Based on the data description identified some columns having mixed data types . So print them to analyze further
 <br>
 5. Create two new columns to store the converted value for below columns to keep data in consistent data type:<br>
 int_rate_numeric: Removed % symbol from int_rate<br>
 empl_length_numeric : Removed the words year and symbols < and > and + from emp_length<br>
 <br>
 6.Identify and handle outliers using IQR for required columns. Here we are considering the below columns<br>
 - loan_amnt<br>
 - annual_inc<br>
 - dti<br>
 - revol_bal<br>
 - total_acc<br>
  <br>
 7.Analyze the Patterns of Loan Defaulters by querying<br>
 -Analyze default rates by loan grade<br>
 -Analyze default rates by employment length<br><br>
 8.Plotted graphs between the below variables for understanding their relation:<br>
   (i)  Loan Status vs Loan Amount<br>
   (ii) Employment Tenure vs Loan Status<br>
   (iii)Home Ownership vs Loan Status<br>
   (iv) Annual Income vs Loan Status<br>
   (v)  Interest Rate vs Loan Status<br>
   (vi) Purpose vs Loan Status<br>
   (vii)Term in months vs Loan Status<br>
   (viii) Grade vs Loan Status<br><br>
 5.Also tried to check the dependency between multi factors:<br>
   (i) Loan amount vs Annual Income, and Loan Status<br>
   (ii) Interest Rate vs Loan Purpose , grouped by Loan Status<br>
