# Bank-Analysis-Tableau--Dashboards
# Tableau Dashboards
<img width="1173" height="588" alt="Bank-analysis-Dashboard-image" src="https://github.com/user-attachments/assets/406c9421-5be4-4866-999a-c7a65d67cd7b" />

Two Tableau workbooks with calculated fields, KPI worksheets and a final dashboard.

---

## 1. Debit & Credit Transaction Analysis
**File:** `DEBIT_AND_CREDIT_BANKING_DATA_1.twbx`

**Goal:** Compare credits against debits, track branch growth and flag high-risk transactions.

**Data:** 100,000 transactions (Jan to Dec 2024, INR), 6 branches, 6 banks, 3 transaction methods.

**Workbook contents:** 14 worksheets combined into **FINAL DASHBOARD**

**Calculated fields**
- Total Credit Amount, Total Debit Amount, Net Transaction Amount
- Credit to Debit Ratio
- Total Transactions, Account Activity Ratio
- Branch Growth %
- High Risk Transaction Flag (amount of ₹4,500 or more)

![Debit & Credit Tableau Dashboard](../images/debit_credit_tableau_dashboard.png)

**Live dashboard:** _add your Tableau Public link here_

### Key Insights
- **Money in and money out are almost perfectly balanced.** Total credits were about ₹127.6M against debits of about ₹127.3M, a net inflow of only about ₹0.32M (roughly 0.25% of credit volume), so the credit-to-debit ratio is close to 1.
- **East Branch had the strongest net inflow (+₹355K), while Main Branch had the largest net outflow (-₹246K).** City Center was also net negative (-₹75K).
- **Net flow swings month to month.** May had the highest net inflow (+₹559K) and April the largest net outflow (-₹513K). Of the 11 full months, 6 were net inflow and 5 net outflow. December has only 305 transactions because the data ends on 1 December, so branch growth for that month is not meaningful.
- **About 10.4% of transactions (10,428) are High Risk.** The flag covers the top slice of an amount range that tops out at about ₹5,000, and the average transaction is about ₹2,549.
- **High-risk share is similar everywhere.** City Center and East Branch are highest at about 11%, the other branches about 10%. By bank, Axis Bank is highest at 10.8% and State Bank of India lowest at 10.2%.
- **Transaction method makes no real difference.** Volume is split evenly (about 33.3K each) and the high-risk share is 10.3% to 10.5% across Bank Transfer, Credit Card and Debit Card.

---

## 2. Bank Loan Portfolio Analysis
**File:** `Tableau_Bank_Analysis_Project.twbx`

**Goal:** Track loan revenue, default and delinquency across the portfolio and by borrower group.

**Data:** About 65.5K loan accounts (FY2017 to FY2020), 16 states, 112 branches, 11 regions, total loan amount of about ₹751M.

**Workbook contents:** 20 worksheets combined into **Dashboard 1**

**Calculated fields**
- Total Revenue (interest received + fees)
- Default Loan Count and Default Loan Rate
- Delinquent Client Count and Delinquent Loan Rate
- Verification Status share
- Age Group (18-25, 26-35, 36-45, 46-55, 56-63)

![Loan Tableau Dashboard](../images/loan_tableau_dashboard.png)

**Live dashboard:** _add your Tableau Public link here_

### Key Insights
- **The portfolio is concentrated geographically.** Uttar Pradesh, Punjab and Bihar make up about 47% of the ₹751M loan value, and the top 5 states about 67%. Ludhiana is the largest region (₹129M).
- **Total revenue (interest + fees) is about ₹156.5M**, roughly 21% of the loan amount.
- **Default Loan Rate is about 1.6%, but Delinquent Loan Rate is about 10.8%.** Delinquency is about 10% to 11% in almost every state, so it is portfolio-wide. Varanasi region is highest at 12%. Chhattisgarh (Raipur region) has the highest default rate among the larger states at about 4%.
- **Credit grade is the strongest risk signal.** Delinquency rises from about 4% for Grade A to 14% (C), 17% (D and E) and 26% (G).
- **Lower grades earn more per rupee lent.** Revenue as a share of loan amount rises from about 10% (Grade A) to about 37% (Grade G).
- **60-month loans drive revenue.** They are about 42% of loan value but about 59% of revenue.
- **Age-group view:** borrowers aged 26 to 45 hold about 67% of loan value. The 56 to 63 group is small but has the highest default rate at roughly 7%, against 1% to 2% elsewhere. Ages 46 to 55 have the highest delinquency at about 12%.
- **Home loans lead** at about 37% of loan value, and the top 3 purposes (Home Loan, Services, Business) make up about 69%.
- **Verification status does not predict risk.** Delinquency is about 11% for Verified, Source Verified and Not Verified loans alike.
- **Borrowers are almost entirely women**, and FY2019 accounts for about 57% of loan value.

## Skills Demonstrated
Calculated fields, KPI design, interactive dashboards, risk and segmentation analysis

## How to Open
Open the `.twbx` files in Tableau Desktop or the free Tableau Public app, or use the live links above.
