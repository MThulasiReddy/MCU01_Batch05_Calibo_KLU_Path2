# 📊 Category Intelligence — Retail Product Performance EDA

### Calibo AI Academy | Phase 1 — Mini Use Case 01

**Category Intelligence — Retail Product Performance EDA**

> An exploratory data analysis project designed to help a Category Manager understand category-level performance, product-level performance, discount patterns, and sales timing before a quarterly supplier review.

---

## 📌 Table of Contents

- [Project Overview](#-project-overview)
- [Business Context](#-business-context)
- [Problem Statement](#-problem-statement)
- [Business Objective](#-business-objective)
- [CBIM Problem Canvas](#-cbim-problem-canvas)
- [Key Business Questions](#-key-business-questions)
- [Dataset Overview](#-dataset-overview)
- [Dataset Structure](#-dataset-structure)
- [Data Dictionary](#-data-dictionary)
- [Data Quality](#-data-quality)
- [Technology Stack](#-technology-stack)
- [Project Architecture](#-project-architecture)
- [Project Workflow](#-project-workflow)
- [Exploratory Data Analysis](#-exploratory-data-analysis)
- [Analysis 1 — Category Revenue Trend](#-analysis-1--category-revenue-trend)
- [Analysis 2 — Product Performance](#-analysis-2--product-performance)
- [Analysis 3 — Discount Effectiveness](#-analysis-3--discount-effectiveness)
- [Analysis 4 — Day-of-Week Analysis](#-analysis-4--day-of-week-analysis)
- [Analysis 5 — Monthly Sales Pattern](#-analysis-5--monthly-sales-pattern)
- [Key Findings](#-key-findings)
- [Category Recommendation](#-category-recommendation)
- [Action Plan](#-action-plan)
- [Risks and Limitations](#-risks-and-limitations)
- [Business Interpretation](#-business-interpretation)
- [Visualizations](#-visualizations)
- [Project Structure](#-project-structure)
- [Installation](#-installation)
- [How to Run](#-how-to-run)
- [Requirements](#-requirements)
- [Expected Output](#-expected-output)
- [Deliverables](#-deliverables)
- [Team](#-team)
- [Future Improvements](#-future-improvements)
- [Conclusion](#-conclusion)

---

# 📌 Project Overview

**Category Intelligence — Retail Product Performance EDA** is a retail analytics project developed as part of the **Calibo AI Academy — Phase 1 Mini Use Case 01**.

The project uses transaction-level retail sales data covering **six months from January to June 2026**.

The objective is to transform raw retail transaction data into meaningful business insights that can help a **Category Manager** prepare for a quarterly supplier review.

The analysis focuses on:

- Category revenue movement
- Product-level performance
- Discount effectiveness
- Day-of-week sales patterns
- Monthly sales patterns
- Category-level recommendation
- Actions for the supplier review

The project follows a business-first EDA approach rather than simply generating charts.

The goal is to answer:

> **Which categories and products are performing well, which are losing momentum, and where should the Category Manager focus attention?**

---

# 🏢 Business Context

The business is a regional retail chain operating across **Andhra Pradesh**.

The chain operates:

- **12 stores**
- **6 cities**
- **5 product categories**
- **25 products**
- **107,836 transactions**
- **6 months of transaction data**

The Category Manager is preparing for a **quarterly supplier review**.

Before the meeting, the manager needs to understand:

1. Which categories are growing?
2. Which categories are declining?
3. Which products are driving each category?
4. Which products are weaker within their categories?
5. Whether deeper discounts are associated with stronger transaction performance?
6. Which days and months show stronger sales performance?
7. What category should receive focused attention?
8. What additional information is needed before making a larger investment decision?

---

# ❗ Problem Statement

A large volume of transaction data is available, but raw transaction records alone do not provide a clear business direction.

The Category Manager needs a concise view of:

- Category momentum
- Product performance
- Discount patterns
- Sales timing
- Business priorities

Without structured analysis, it becomes difficult to identify which categories require attention before the supplier review.

Therefore, the project converts transaction-level data into category-level and product-level business insights.

---

# 🎯 Business Objective

The primary objective is:

> **To analyze six months of retail transaction data and identify category and product performance patterns that can support the Category Manager during the quarterly supplier review.**

The analysis specifically aims to:

### 1. Understand Category Momentum

Identify which categories are growing or declining from January to June 2026.

### 2. Identify Product Leaders and Laggards

Find the highest- and lowest-revenue products within each category.

### 3. Examine Discount Effectiveness

Compare average revenue per transaction across different discount brackets.

### 4. Understand Sales Timing

Analyze average revenue per transaction by day of week and total revenue by month.

### 5. Provide One Clear Recommendation

Convert the analysis into one category-level recommendation supported by the observed data.

---

# 🧩 CBIM Problem Canvas

The business problem was defined using the **CBIM Problem Canvas** before starting the analysis.

## Situation

A regional retail chain has 12 stores across 6 cities and is preparing for a quarterly supplier review. The Category Manager has six months of sales data across five product categories.

## Complication

The manager needs to quickly understand which categories and products are performing well, which are losing momentum, and where attention is needed.

## Question

Which categories and products are performing well or declining, and where should the Category Manager focus attention?

## SSOT — Single Source of Truth

The six-month retail transaction dataset covering:

**January 2026 → June 2026**

## Success Definition

The analysis should provide clear evidence about category and product performance and lead to one clear category-level recommendation for the supplier review.

## Primary Stakeholder

**Category Manager**

The Category Manager needs clear priorities and evidence to support the quarterly supplier discussion.

---

# ❓ Key Business Questions

The analysis is structured around five major questions.

### Question 1 — Category Momentum

> Which product categories are growing or declining month-on-month?

### Question 2 — Product Performance

> Which products are leading or lagging within each category?

### Question 3 — Discount Effectiveness

> Do deeper discounts correspond with stronger transaction performance?

### Question 4 — Sales Timing

> When does the retail chain perform best across days and months?

### Question 5 — Category Decision

> What single category-level recommendation should follow from the evidence?

---

# 📊 Dataset Overview

The project uses the simulated retail transaction dataset:

```text
MUC01_Retail_Sales_Dataset.csv
