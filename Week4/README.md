
# Week 4 - Cohort Analysis and Advanced Business Analysis

## Overview
Superstore dataset analysis for NexAfrica Internship.

Files:
- `Cohort Analysis And Advanced Business Analysis.xlsx` - All pivots
- `Cohort and Advanced Business Analysis Report.docx` - Full report

## Part A - Cohort Analysis
- Q1 New: Jan 79, Feb 41, Mar 147 (Peak March)
- Q2 Revenue: 2014-03 highest ~$3,288
- Q3 Strongest: 2014-02 = 24% retention (10/41) vs avg 6%
- Q4 Trend: 100% M0 -> 6-24% M1 -> 0% M3+ = one-time buyers
![Cohort %](Screenshot%202026-10-01%20133629.png)

## Part B - Discount Analysis
- Highest: Binders 37.23%, Machines 30.61%, Tables 26.13%
- Avg 15.62%
- Impact: 0%=66.89, 10%=96.05 peak, 30%=-45.67 LOSS, 45%=-226.64
- Cap at 20%, optimal 10%
![Discount](Screenshot%202026-10-01%20150249.png)
![Discount vs Profit](Screenshot%202026-10-01%20150316.png)

## Part C - Profitability
- STARS: Accessories 41,527 profit, Phones 44,515, Chairs 26,590
- PROBLEM: Tables 333 sales / -17,725 loss, Bookcases -3,472
- NICHE: Copiers 55,617 profit
- Grand Total: 285,988
![Profitability](Screenshot%202026-10-01%20150231.png)
![Summary](Screenshot%202026-10-01%20150334.png)

## Key Findings
1. Retention crisis 94% never return
2. Feb 2014 best cohort 24%
3. Discount >30% = loss
4. Phones/Accessories = 70% profit
5. Tables = net loss -17k

## Recommendations
1. Cap discount 20% max
2. Remove discount on Tables/Binders
3. Launch Month 1 retention email
4. Focus on Phones, Chairs, Accessories
5. Replicate Feb 2014 channel

## Fix Applied
SA locale fix: Replaced `.` with `,` in Sales/Discount/Profit columns to fix #DIV/0! and inflated 3723% issue.
