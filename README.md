# Personalization Impact Analysis: Marketing Analytics

Analyzed a randomized marketing experiment for a European book retailer to understand how personalized recommendations affect customer purchases. Compared generic and personalized letters across four lifecycle segments to identify opportunities for reactivation and more effective targeting.

---

## Project Motivation

Determine which customers respond to personalized recommendations and whether personalization increases purchase rates, order size, and spending.

---

## Data Overview

| Dataset | Description |
| --- | --- |
| `book.csv` | Customer-level results from a randomized catalog personalization experiment. |

### Unit of Analysis

- 115,962 customer records
- Control group received generic recommendations
- Treatment group received personalized recommendations

### Customer Segments

- **New:** Customers acquired in the past year
- **Active:** Established customers who purchased in the past year
- **Recently lapsed:** Customers who purchased in the previous year
- **Long lapsed:** Customers who had not purchased in at least two years

### Key Variables

- **tx:** Generic letter (0) or personalized letter (1)
- **RFseg:** Customer lifecycle segment
- **buy:** Whether the customer placed an order
- **totitem:** Number of items ordered
- **toteuro:** Order amount in euros

---

## Methodology

1. **Test versus control comparison** to measure purchase-rate differences within each segment
2. **Order analysis** to compare items purchased and spending among buyers
3. **Financial assessment** to explore revenue implications for targeted personalization

---

## Key Findings

- Personalized recommendations increased purchase rates among recently and long-lapsed customers.
- Recently lapsed purchase rates rose from **2.78% to 3.41%**; long-lapsed rates rose from **1.08% to 1.67%**.
- Purchase-rate differences for new and active customers were not statistically significant at the 5% level.
- Among long-lapsed buyers, average order size was **4.35 items with generic recommendations versus 5.61 with personalization**.

The results support prioritizing lapsed customers for further personalization testing. Comparisons among buyers describe those who purchased; they do not isolate the effect on order size for the same customers. 

---

## Key Methods & Tools

| Category | Details |
| --- | --- |
| Methods | Randomized experiment analysis, proportion tests, Welch's t-tests, lifecycle segmentation |
| Tools | R / RStudio for the class project; Python for an independent check of the supplied data |

---

## How to Run

The original R script is not included. This README summarizes the group project and findings checked against `book.csv`; runnable analysis code can be added separately.

---

*Northwestern University, IMC460: Data Science. Group project by Ina Lin, Cindy Chou, Khwaish Gohil, Yin Zhi, and Priya Thakore.*
