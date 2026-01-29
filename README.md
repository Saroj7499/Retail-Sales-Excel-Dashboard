# Sales Distribution & Seasonal Analysis Dashboard (Excel Project)

## Project Overview
This project is an end-to-end Excel data analysis and dashboarding project built from raw retail transaction data.The objective was not just to create charts, but to think like a data analyst — cleaning data, engineering new columns, validating logic, and finally building insight-driven dashboards.

The project evolved in multiple stages, starting from raw transaction tables to multiple analytical sheets and finally an interactive dashboard.

## Dataset Description
**File Name:** PNRao_SalesRetail_Sales_Transactions.xlsx

The base dataset contains transaction-level retail sales data with the following core fields:
- TransactionID
- Date
- CustomerID
- StoreID
- EmployeeID
- PromotionID
- PaymentMethod
- TotalAmount

# Data Preparation & Feature Engineering
Before analysis, the raw data was enhanced by creating additional columns:

- **Month Number** (derived from Date)
- **Month Name** (January, February, etc.)
- **Season** (Makar Sankranti / Regular)
- **Promo Flag** (Promoted / Not Promoted)
- **Employee Known Flag** (Known Employee / Unknown Employee)
- **Customer Visit Count** (repeat visits per customer)

## Sheets & Analysis Breakdown
 ### 1.Sales_Transactions (Raw Data Sheet)
- Original transaction-level data
- Used as the single source of truth for all pivot tables

## 2. Transaction_working (Data Enrichment Sheet)
- Created calculated columns using formulas such as:
    - IF conditions for Known vs Unknown Employee
    - Month extraction and naming
- Acts as a cleaned and modeled dataset for analysis

This mirrors a real-world data modeling step before BI reporting.

## 3. Total Sales Summary
- Pivot table to calculate **Total Revenue**
- **Total Sales:** ₹268,788.4

## 4. Store Contribution Analysis

**Sheet:** Store contribution
- Revenue contribution by each store (STO-01 to STO-04)
- **Top Store:** STO-04

Helps management identify high-performing locations.

## 5. Employee Type Contribution

**Sheet:** Employee type

Employee Type	          Revenue Share
Known Employee	            ~96.7%
Unknown Employee	          ~3.3%

Indicates that tracked employees drive most revenue.

## 6. Promotion vs Non-Promotion Analysis

**Sheet:** promo vs noprom

Category	            Revenue
Promoted	            ₹259,620.3
Not Promoted	        ₹9,168.1

Strong evidence that promotions are a major revenue driver.

## 7. Promotion Impact Analysis

**Sheet:** promotion impact
Compared **Total Revenue** and **Average Order Value**

Category             	Avg Order Value
Promoted                  	~₹336
Not Promoted              	~₹286

Promotions increase volume more than ticket size.

## 8. Monthly Sales Trend

**Sheet:** monthly_sales
- Month-wise sales trend analysis
- Peak Month: July

 Reveals seasonality patterns in sales.

## 9. Highest Seasonal Sale

**Sheet:** Highest Seasonal Sale
- Analyzed sales based on Season
- Compared festive period (Makar Sankranti) vs regular days

Shows how seasonal events impact customer spending.

## 10. Most Valuable Customer

**Sheet:** most valuable custo
Identified customer contributing the highest total revenue
**Top Customer:** CUST-1196

Useful for loyalty programs and targeted marketing.

## Interactive Dashboard

**Sheet:** Dashboard
A consolidated dashboard combining all key insights:
- KPI Cards:
   - Total Revenue
   - Top Store
   - Best Month
   - Top Customer
- Store Contribution Chart
- Promotion Impact Chart
- Employee Type Contribution Chart
- Monthly Sales Trend

## Slicers Used
- Month
- Store ID
- Promotion Flag

All visuals respond dynamically to slicer selections.

## Tools & Techniques Used
- Microsoft Excel
- Pivot Tables & Pivot Charts
- Advanced Excel formulas (IF, MONTH, TEXT)
- Data modeling using helper columns
- Slicers for interactivity
- Dashboard layout & formatting

## Key Business Insights
- STO-04 is the highest revenue-generating store
- Promotions drive the majority of sales revenue
- Known employees contribute nearly all revenue
- July is the peak sales month
- Festive seasons show higher spending behavior
- A small set of customers contribute disproportionately to revenue

## How to Use

1. Download the Excel file
2. Enable content if prompted
3. Navigate to the Dashboard sheet
4. Use slicers to explore different scenarios

## Future Enhancements

- Profit & margin analysis
- RFM customer segmentation
- Power Query automation
- Migration to Power BI
