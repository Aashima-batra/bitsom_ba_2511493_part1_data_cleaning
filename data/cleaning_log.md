# Data Cleaning Log

## Project
Order Data Cleaning and Quality Assessment

---

## Issues Identified

The following data quality issues were identified during the data cleaning process:

- Missing values in selected categorical fields
- Exact duplicate records
- Duplicate Order IDs
- Mixed date formats in Order Date and Ship Date
- Invalid discount values (negative and above business limit)
- Ship Date occurring before Order Date
- Sales calculation inconsistencies
- Profit calculation inconsistencies
- Inconsistent text formatting
- Order and payment status inconsistencies

---

## Cleaning Actions Performed

The following cleaning activities were completed:

- Removed exact duplicate records.
- Standardized text fields using TRIM and PROPER functions where applicable.
- Standardized Order Date and Ship Date into a consistent date format.
- Validated shipping dates against order dates.
- Standardized discount values based on business rules.
- Created calculated sales and calculated profit columns for validation.
- Calculated shipping delay in days.
- Calculated profit margin.
- Added validation and flag columns for data quality checks.
- Standardized payment status and order status values.
- Reviewed missing values and replaced categorical blanks with "Unknown" where applicable.

---

## Business Rules Applied

The following business rules were applied during cleaning:

- Order ID must be unique.
- Ship Date must not occur before Order Date.
- Discount values must fall within the acceptable business range.
- Sales should equal Quantity × Unit Price × (1 − Discount).
- Profit should equal Sales − Cost.
- Missing categorical values should be replaced with "Unknown" where appropriate.
- Date fields must contain valid Excel dates.
- Text values should use consistent capitalization and formatting.

---

## Assumptions Made

- Duplicate Order IDs with different transaction details were treated as valid business transactions.
- Missing categorical values were replaced with "Unknown" when the original value could not be determined.
- Minor calculation differences caused by decimal rounding were considered acceptable.
- Existing sales and profit values were assumed to be correct unless validation identified a mismatch.

---

## Records Removed

- Exact duplicate records removed: **20**

---

## Records Flagged

The following records were flagged for review:

- Invalid shipping dates
- Discount validation issues
- Sales calculation mismatches
- Profit calculation mismatches
- Duplicate Order IDs requiring business verification

---

## Limitations

- Business validation was limited to the available dataset.
- Product pricing and cost values could not be verified against external systems.
- Duplicate Order IDs may represent legitimate repeat transactions.
- Missing values were handled using business assumptions where necessary.

---

## Conclusion

The dataset was successfully cleaned, standardized, validated, and prepared for business reporting and dashboard development.