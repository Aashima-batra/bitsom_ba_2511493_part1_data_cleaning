# Order Data Cleaning & Data Quality Assessment (Part 3)

## Project Summary

This project focuses on cleaning, validating, and assessing the quality of an order dataset using Microsoft Excel. The objective was to improve data accuracy, identify quality issues, apply business validation rules, and generate summary reports to support business analysis.

---

# Dataset Description

The dataset contains customer order information, including:

- Order ID
- Order Date
- Ship Date
- Customer Information
- Region
- State
- City
- Category
- Sub Category
- Product Name
- Ship Mode
- Quantity
- Unit Price
- Discount
- Sales
- Cost
- Profit
- Payment Status
- Order Status

Additional calculated columns were created during the cleaning process.

---

# Tools Used

- Microsoft Excel
- Excel Functions
- Pivot Tables
- Conditional Formatting
- Data Validation
- Formula-based Quality Checks

---

# Data Cleaning Steps

The following cleaning tasks were completed:

- Removed duplicate records
- Standardized text values
- Cleaned inconsistent date formats
- Validated shipping dates
- Checked missing values
- Validated discount values
- Calculated shipping delay
- Calculated sales
- Calculated profit
- Calculated profit margin
- Standardized payment status
- Standardized order status
- Created validation and quality flag columns

---

# Business Rules Applied

- Order ID should be unique.
- Ship Date cannot occur before Order Date.
- Discount values must remain within the accepted business range.
- Sales = Quantity × Unit Price × (1 − Discount)
- Profit = Sales − Cost
- Missing categorical values were replaced with "Unknown" where appropriate.

---

# Data Quality Issues Found

The following issues were identified:

- Missing values
- Duplicate records
- Duplicate Order IDs
- Mixed date formats
- Invalid shipping dates
- Discount validation issues
- Sales calculation mismatches
- Profit calculation mismatches
- Text formatting inconsistencies

---

# Data Quality Report

The report includes:

- Missing Value Summary
- Duplicate Summary
- Invalid Discount Summary
- Date Issue Summary
- Order Status Issue Summary
- Sales & Profit Calculation Mismatch Summary
- Final Clean vs Flagged Record Count

---

# Pivot Summary Report

The Pivot Summary Report includes:

- Sales and Profit by Region
- Sales and Profit by Category and Sub Category
- Order Count by Ship Mode
- Profit Margin by Customer Segment
- Refunded / Cancelled / Failed Orders by Region
- Monthly Sales Trend

Two pivot reports include sorting and filtering to improve readability.

---

# Key Business Insights

- Regional sales performance varies significantly across regions.
- Technology and Furniture categories contribute a major share of sales.
- Standard Class is the most frequently used shipping mode.
- Customer profitability differs across customer segments.
- Refunded and cancelled orders are concentrated in selected regions.
- Monthly sales trends help identify seasonal business performance.

---

# Assumptions

- Duplicate Order IDs may represent valid repeat business.
- Missing categorical values were replaced with "Unknown".
- Small calculation differences due to decimal rounding were accepted.

---

# Limitations

- Analysis is based only on the provided dataset.
- External validation of product pricing and costs was not available.
- Some business assumptions were required for incomplete records.

---

# Repository Structure

```
raw_data/
outputs/
screenshots/
README.md
```

---

# Screenshots Included

- raw_data_preview.png
- cleaned_data_preview.png
- pivot_summary_1.png
- pivot_summary_2.png

---

# Final Output

The dataset has been successfully cleaned, validated, and summarized for business analysis. Data quality reports and pivot summaries provide meaningful insights for decision-making while improving the reliability of the dataset.
