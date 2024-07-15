# LendingClubCaseStudy
<br>
<br>
## Steps taken for the analysis
<br><br>
 1.Removed the columns in loan.csv which were having NULL for all rows starting from column name 'annual_inc_joint'<br><br>
 2.Removed columns which could not add a pointer for analysis OR  all rows had same values in these columns:
 -ID
 -Member-Id
 -emp_title 
 -url
 -zip_code
 -mths_since_major_derog
 -application_type
3. Removed employment tenure having values N/A
and removed '+' , '<' characters from this column, to consider it as number type 

 
 2.Renamed a few columns for purpose of understanding while querying<br><br>
  term --> term_in_months<br>
  emp_tenure --> employment_tenure_of_borrower_years<br>
 3.Removed outliers using Interquartile Range method<br><br>
 4. Plotted graphs between the below variables for understanding their relation:<br>
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
