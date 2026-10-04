# Power Query Data Cleaning Process

## Overview

Microsoft Excel Power Query was used to clean, transform, standardize, and validate the 5,000-row e-commerce dataset before analysis.

The cleaning process was guided by the business questions defined at the beginning of the project. This ensured that fields required for sales, product, geographic, and delivery analysis were prepared appropriately.

The objective was not simply to remove problematic records. Where possible, the original records were retained while validation and clean analytical fields were created.

---

## 1. Initial Data Profiling

Before applying transformations, I reviewed the dataset using Power Query's data profiling features.

I checked:

- Column data types
- Column quality
- Valid values
- Errors
- Empty/null values
- Distinct values
- Value distributions
- Formatting inconsistencies
- Potential outliers

This assessment helped identify the transformations and validation rules required for each field.

---

## 2. Order ID Validation

The Order ID field was checked for:

- Missing values
- Blank values
- Invalid IDs
- Duplicate IDs

A validation/status field was created to distinguish valid and missing Order IDs.

### Result

- 4,960 Valid
- 40 Missing
- No duplicate Order IDs identified

---

## 3. Customer Name Cleaning

Customer names contained formatting problems including unwanted special characters and inconsistent text.

Power Query text transformations were used to clean and standardize the field.

The column was also checked for missing values.

---

## 4. Customer Email Validation

Customer Email contained valid, invalid, and missing email addresses.

Examples of problematic formats included:

- Missing `@`
- Multiple `@` symbols
- Incomplete addresses
- Missing values

An Email Status field was created to classify records.

### Result

- 4,909 Valid
- 88 Invalid
- 3 Missing

---

## 5. Gender Standardization

Gender contained inconsistent capitalization such as:

- `female`
- `Female`
- `FEMALE`
- `male`
- `Male`
- `MALE`

Text formatting was standardized so equivalent values were grouped consistently.

Missing values were handled as `Unknown`.

### Final Categories

- Male
- Female
- Unknown

---

## 6. Age Validation

Age was converted to an appropriate numeric data type and checked for unrealistic values.

Values included negative ages, zero, extreme ages, and missing records.

A validation field was created using an acceptable analytical range of 18–70 years.

### Result

- 4,899 Valid
- 98 Invalid
- 3 Missing

---

## 7. Country and City Cleaning

Country names contained inconsistent capitalization and missing values.

Country text was standardized so equivalent country names could be grouped correctly during geographic analysis.

Missing countries were handled consistently.

The City field was also profiled for completeness.

### Data Quality Observation

- Country: 41 missing values originally identified
- City: 46 missing values identified

---

## 8. Product Category Standardization

Product Category contained inconsistent capitalization and missing categories.

The field was standardized into consistent category names.

Missing categories were classified as `Unknown`.

### Final Categories

- Beauty
- Electronics
- Fashion
- Home Appliances
- Unknown

This prevented missing categories from appearing as unexplained `(blank)` values in the final analysis.

---

## 9. Product Name Validation

Product Name was reviewed for consistency and missing values.

### Data Quality Observation

- 44 missing product names identified

Missing records were tracked rather than automatically deleting the associated transactions.

---

## 10. Quantity Cleaning and Validation

Quantity contained several data-quality problems, including:

- Text mixed with numbers, such as `1 units`
- Negative quantities
- Zero quantities
- Extreme quantities/outliers
- Type-conversion issues

The field was cleaned and converted to numeric form.

A validation field was then created to distinguish valid, invalid, and outlier quantities.

### Result

- 4,921 Valid
- 48 Invalid
- 31 Outliers
- 0 Missing

---

## 11. Unit Price Cleaning

Unit Price contained inconsistent numeric and currency representations.

Currency text/symbols were removed where necessary and the field was converted to a numeric data type.

The cleaned field was checked for errors and missing values.

### Result

- No errors
- No blanks after cleaning

---

## 12. Discount Rate Validation

The Discount field was standardized as a decimal field and validated using Power Query's column profiling tools.

### Valid Discount Rates

- 0
- 0.05
- 0.10
- 0.15
- 0.20
- 0.25

### Result

- No errors
- No blanks

---

## 13. Total Sales Validation

Recorded Total Sales values were checked against calculated transaction values.

A validation process was used to distinguish:

- Valid
- Mismatch
- Not Validated

This helped prevent questionable sales values from being silently included in the final analysis.

### Result

- 4,831 Valid
- 90 Mismatch
- 79 Not Validated

---

## 14. Clean Total Sales

A separate `Clean Total Sales` field was prepared for analytical calculations.

Only transactions meeting the required validation conditions were included in the clean analytical sales measure.

### Result

- 4,921 valid analytical sales values
- 79 null
- 0 errors

The final dashboard and sales analysis were based on the cleaned analytical sales field.

---

## 15. Payment Method Standardization

Payment Method values were reviewed and standardized so equivalent payment methods were grouped consistently.

Final categories included:

- Mobile Money
- Bank Transfer
- Credit Card
- Cash on Delivery
- Debit Card
- PayPal
- M-Pesa
- Cash

---

## 16. Order Date Standardization

Order Date contained multiple date representations.

The values were standardized and converted into an appropriate date data type.

The cleaned dates were then checked for conversion errors and missing values.

### Result

- 5,000 records
- 0 errors
- 0 empty values

This field was required for the monthly sales trend analysis.

---

## 17. Shipping Date Standardization

Shipping Date also contained inconsistent date representations.

The field was standardized and converted to an appropriate date format before calculating shipping duration.

### Result

No errors, blanks, or null values remained after standardization.

---

## 18. Shipping Days Calculation

A Shipping Days field was calculated from the difference between Shipping Date and Order Date.

The resulting values were profiled to identify missing values and unusually long shipping periods.

### Result

- 4,981 Valid
- 19 Null
- 0 Errors
- Minimum: 1 day
- Maximum: 244 days
- 18 outliers identified

---

## 19. Delivery Status Standardization

Delivery Status was cleaned and standardized so equivalent labels were grouped correctly.

Missing delivery statuses were classified as `Unknown`.

### Final Categories

- Returned
- Cancelled
- Processing
- Delivered
- Shipped
- Unknown

---

## 20. Customer Rating Validation

Customer Rating contained numeric ratings, text representations, invalid values, and missing values.

Valid ratings were standardized to a numeric 1–5 scale.

A validation/status field was created to distinguish valid, invalid, and missing ratings.

### Result

- 4,926 Valid
- 47 Invalid
- 27 Missing

Only valid ratings were used for the clean customer-rating analysis.

---

## 21. Final Data-Type Review

After cleaning, the data types were reviewed and assigned according to analytical purpose.

These included:

- Text
- Whole Number
- Decimal Number
- Date/Date-Time

This ensured that calculations, PivotTables, grouping, and dashboard filters worked correctly.

---

## 22. Final Quality Check

Before loading the dataset for analysis, I reviewed:

- Row count
- Column quality
- Errors
- Missing values
- Validation fields
- Clean analytical fields
- Data types
- Duplicate Order IDs

The original dataset contained 5,000 rows, and all 5,000 source records were retained after the cleaning and validation process.

Problematic values were identified through validation fields rather than automatically removing entire records.

---

## Final Output

The cleaned dataset was loaded into Excel and used to build:

- PivotTable analysis
- KPI calculations
- Monthly sales analysis
- Product-category analysis
- Product-level analysis
- Country analysis
- Delivery-status analysis
- Customer-rating analysis
- Interactive dashboard

The complete detailed record of identified issues, cleaning actions, validation rules, and results is available in `cleaning_log.xlsx`.