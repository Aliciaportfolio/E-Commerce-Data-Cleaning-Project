# E-Commerce Data Cleaning Project

## Objective
Clean and prepare raw e-commerce sales data for analysis in Power BI.

## Dataset Overview
- **Rows**: 1,200 orders
- **Columns**: OrderID, Date, CustomerID, Product, Quantity, UnitPrice, ShippingAddress, PaymentMethod, OrderStatus, TrackingNumber, ItemsInCart, CouponCode, ReferralSource, TotalPrice
- **Date Range**: 2023-2025

## Cleaning Steps Applied
1. Promoted Headers
2. Changed Type - set:
   - IDs (ID, CustomerID, TrackingNumber) → Text
   - Dates → Date 
   - Text fields (Product, ShippingAddress, PaymentMethod, OrderStatus, CouponCode, ReferralSouce ) → Text
   - Numeric (Quantity, ItemsInCart) → Whole Number
   - Monetary (UnitPrice, TotalPrice) → Currency
3. Removed Blank Rows
4. Removed Duplicates
5. Filtered Rows - removed test orders
6. Trimmed Text - cleaned Product and ShippingAddress fields

## Key Transformations
- Standardized CouponCode: SAVE10, FREESHIP, NONE
- Unified ReferralSource: Instagram, Facebook, Email, Google, Referral
- Validated TotalPrice range: $11.39 - $3,460

## Files
- `data/sales_data_cleaned.csv` - Final cleaned dataset
- `scripts/cleaning_steps.txt` - Detailed Power Query M code
- `screenshots/CLEANED_DATASET.png` - Preview of final table# E-Commerce-Data-Cleaning-Project
