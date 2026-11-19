# Bank Loan Report — SQL & Power BI Portfolio Analysis

An end-to-end banking analytics project that tracks loan applications, funded capital, borrower repayments, and credit risk across **38,576 loan applications** using **SQL Server** for data validation and **Power BI** for interactive reporting.

---

## Project Objective

Build a three-page Bank Loan Report to monitor lending volume, cash flow, and portfolio quality:
1. **Summary Dashboard:** Track top-line Key Performance Indicators (KPIs), Month-to-Date (MTD) and Month-over-Month (MoM) trends, Good Loan vs. Bad Loan performance, and Loan Status metrics.
2. **Overview Dashboard:** Analyze lending patterns by month, state, loan term, employment length, loan purpose, and home ownership.
3. **Details Dashboard:** Provide a filterable, loan-level table for inspecting individual borrower accounts by state, credit grade, and purpose.

---

## Key Portfolio Metrics (Verified in SQL & Power BI)

| Metric | Overall | MTD (December) | PMTD (November) | MoM Change |
| :--- | ---: | ---: | ---: | ---: |
| **Total Loan Applications** | 38,576 | 4,314 | 4,035 | +6.9% |
| **Total Funded Amount** | $435,757,075 | $53,981,425 | $47,754,825 | +13.0% |
| **Total Amount Received** | $473,070,933 | $58,074,380 | $50,132,030 | +15.8% |
| **Average Interest Rate** | 12.05% | 12.36% | 11.94% | +3.5% |
| **Average Debt-to-Income (DTI)** | 13.33% | 13.67% | 13.30% | +2.7% |

### Good Loans vs. Bad Loans

| Category | Loan Status Included | Applications | Share | Funded Amount | Amount Received |
| :--- | :--- | ---: | ---: | ---: | ---: |
| **Good Loans** | Fully Paid, Current | 33,243 | 86.2% | $370,224,850 | $435,786,170 |
| **Bad Loans** | Charged Off | 5,333 | 13.8% | $65,532,225 | $37,284,763 |

---

## Key Findings

* **Net Positive Overall Recovery:** Total repayments ($473.1M) exceeded total funded principal ($435.8M) by **+$37.3M** (108.6% recovery), driven by Good Loans returning $65.6M above principal.
* **Unrecovered Principal in Bad Loans:** Charged Off loans (5,333 accounts) returned only 56.9% of funded principal, leaving **$28.2M unrecovered**. Charged Off loans also had higher average interest rates (13.88%) and DTI (14.00%) than Fully Paid loans (11.64% rate, 13.17% DTI).
* **Elevated Risk in Current Loans:** The 1,098 active Current loans ($18.9M funded) carry the highest average interest rate (15.10%) and DTI (14.72%) in the portfolio, making them a priority for early-warning monitoring.
* **Strong Year-End Growth:** Monthly applications rose **85.0%** from January (2,332) to December (4,314), while monthly funded volume more than doubled (+115.7%, from $25.0M to $54.0M).
* **Segment Concentration:** **Debt consolidation** drives 47.2% of all applications (18,214 loans), **36-month terms** account for 73.2% of loans, and **California** (6,894), **New York** (3,701), and **Florida** (2,773) lead state volume.
* **Small Business Shortfall:** Out of all 14 loan purposes, **small business** (1,776 loans) is the only category where repayments ($23.81M) fell below funded principal ($24.12M)—a net shortfall of **-$308K**.

---
