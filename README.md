```markdown
# Category Intelligence — Retail Product Performance EDA

## Overview

Category Intelligence is a retail analytics project designed to help a Category Manager understand product and category performance before a supplier review.

The project analyzes six months of retail transaction data from January 2026 to June 2026 across multiple stores, cities, products, and categories.

The analysis focuses on identifying:

- Categories with positive or negative momentum
- Product-level performance
- Revenue concentration
- Discount and transaction-value patterns
- Monthly and day-of-week trends
- Locations and products suitable for controlled business tests
- Data required for stronger profitability decisions

## Business Problem

A regional retail chain operates 12 stores across 6 cities in Andhra Pradesh and sells products across five categories:

- Electronics
- Apparel
- Grocery
- Home & Kitchen
- Personal Care

The Category Manager needs evidence to understand:

1. Which categories are performing well?
2. Which categories require attention?
3. Which products are contributing strongly to revenue?
4. How are categories changing over time?
5. How are discounts associated with transaction revenue?
6. Where should promotion or discount tests be considered?
7. What additional data is needed before making profitability decisions?

## Objective

The objective is to provide an evidence-based view of category and product performance that can support supplier discussions, category reviews, promotion testing, and business planning.

## Dataset

The analysis uses six months of retail transaction data covering:

- **107,836 transactions**
- **25 products**
- **5 categories**
- **12 stores**
- **6 cities**
- **January 2026 to June 2026**
- **₹459.8M observed post-discount revenue**

The original dataset contains 10 fields and no missing values.

## Dataset Fields

| Field | Description |
|---|---|
| `transaction_id` | Unique transaction identifier |
| `date` | Transaction date |
| `store_id` | Store identifier |
| `store_city` | City of the store |
| `category` | Product category |
| `product_name` | Product name |
| `units_sold` | Number of units sold |
| `unit_price` | Price per unit |
| `revenue` | Revenue generated from the transaction |
| `discount_pct` | Discount percentage |

## Key Findings

### Category Performance

| Category | January → June |
|---|---:|
| Apparel | +34.1% |
| Personal Care | +2.2% |
| Grocery | -3.6% |
| Home & Kitchen | -18.5% |
| Electronics | -35.0% |

### Revenue Concentration

Electronics represents **49.3% of observed revenue**.

Despite being the largest revenue category, Electronics declined by **35.0%** from January to June.

### Apparel

Apparel increased by **34.1%** from January to June.

The growth is broad across products rather than being dependent on a single product.

### Electronics

All five Electronics products declined from January to June:

| Product | Change |
|---|---:|
| Headphones | -20.3% |
| Laptop | -30.7% |
| Mobile Phone | -57.1% |
| Smart TV | -21.9% |
| Tablet | -41.0% |

Mobile Phone recorded the largest decline at **57.1%**.

## Discount Analysis

Average revenue per transaction across discount levels:

| Discount | Average Revenue per Transaction |
|---:|---:|
| 0% | ₹4,685.65 |
| 5% | ₹4,300.00 |
| 10% | ₹4,010.00 |
| 15% | ₹4,070.00 |
| 20% | ₹3,631.73 |

Average units remained almost unchanged:

- 0% discount: **2.59 units**
- 20% discount: **2.58 units**

The discount analysis is observational. It shows an association between discount levels and transaction revenue, but it does not establish that discounts caused the change.

## Time-Based Findings

### Day of Week

Saturday recorded the highest average transaction revenue:

**₹4,420.02**

### Month

January recorded the highest total revenue:

**₹84.77M**

## Location-Level Findings

### Tirupati — Apparel

Tirupati recorded **58.5% Apparel growth**, making it a useful location for a controlled Apparel promotion test.

### Guntur — Electronics

Guntur recorded a **44.9% Electronics decline**, making it a useful location for a targeted Electronics test.

## Business Recommendations

### Apparel

Use Apparel as a potential controlled growth-investment case because of its **34.1% January-to-June growth** and broad product participation.

### Electronics

Review Electronics through a supplier recovery discussion because of its **35.0% decline**, large **49.3% revenue share**, and decline across all five products.

### Home & Kitchen

Review product-level performance because the category declined by **18.5%**.

### Grocery and Personal Care

Continue regular monitoring because their changes were smaller:

- Grocery: **-3.6%**
- Personal Care: **+2.2%**

### Promotions and Discounts

Use targeted testing rather than assuming that deeper discounts automatically create stronger demand.

A suitable approach is:

**Test → Measure → Learn → Scale**

## Suggested Controlled Tests

### Apparel Promotion Test

- **Location:** Tirupati
- **Category:** Apparel
- **Initial timing:** Saturday

The purpose is to measure incremental revenue rather than simply total sales.

### Electronics Discount Test

- **Location:** Guntur
- **Category:** Electronics
- **Product:** Smart TV
- **Initial timing:** Tuesday / weaker-demand window

Margin and inventory information should be reviewed before applying deep discounts.

## Limitations

The dataset does not include:

- Product cost
- Gross margin
- Inventory levels
- Stockout history
- Promotion campaign identifiers
- Promotion exposure
- Promotion funding

Because cost and margin data are unavailable, the analysis does not determine profitability.

Because discount data is observational, the analysis does not establish causal impact.

## Additional Data Required

For stronger business decisions, the following data would be useful:

- Product cost
- Gross margin
- Inventory levels
- Stockout history
- Promotion exposure
- Campaign identifiers
- Promotion funding

## Business Decision Framework

The project follows a simple decision framework:

**Invest where positive momentum exists.**

**Challenge material declines.**

**Test before scaling.**

**Measure incremental impact.**

**Check profitability before making larger decisions.**

## Team

| Team Member | Role |
|---|---|
| Thulasi Reddy | Business Analyst & Recommendations |
| Pratik Pattewar | Data Visualization & Insights |
| Dhanesh | Data Analyst & EDA |

## Project Information

**Project:** Category Intelligence  
**Use Case:** Retail Product Performance  
**Analysis Type:** Exploratory Data Analysis  
**Data Period:** January 2026 – June 2026  
**Transactions:** 107,836  
**Products:** 25  
**Categories:** 5  
**Stores:** 12  
**Cities:** 6  
**Region:** Andhra Pradesh
```
