# [Customer credit card behavior analysis]
  This is my first SQL project. I created the schema with synthetic credit card information to practice what I've learned up to this point.  

---

## ⚙️ Project Type Flags

- [x] SQL Analysis / Querying

---

## Table of Contents
1. [Objectives](#1-objectives)
2. [Project Tools](#2-project-scope--tools)
3. [Data Model & Schema](#3-data-model--schema)
4. [Analysis & Metrics](#4-analysis--metrics)
5. [Author](#5-author)

---

## 1. Objectives

<!--
  Write objectives that are specific enough to succeed or fail.
  Use action-oriented verbs: Identify, Determine, Quantify, Build, Evaluate.

  WHAT GOOD LOOKS LIKE:
  ✅ "Determine whether customer churn rate correlates with support ticket volume."
  ✅ "Identify the top three revenue-driving product categories across all regions."
  ✅ "Build a reproducible pipeline that ingests and cleans daily sales exports."

  WHAT TO AVOID:
  ❌ "Explore the data."
  ❌ "Gain insights."
  ❌ "Understand trends."
  (These can't fail - which means they can't succeed either.)
-->

- **Primary Objective:** [Practice SQL queries using joins, cte's, subqueries, window functions, ect.]

---

## 2. Project Tools

### Tools & Technologies

<!--
  List only what you actually used on this project.
  This is not your skills section - it's the project's technical context.
-->

| Category | Tool(s) Used |
|----------|-------------|
| Data Storage | [MySQL] |
| Data Processing | [SQL] |
| Analysis | [SQL queries] |


---

## 3. Data Model & Schema

<!--
  Define your fields so that someone reading your analysis can follow along
  without digging through your code.

  WHAT GOOD LOOKS LIKE (one row example):
  | transaction_id | string | Unique identifier per sales transaction | TXN-00482 |
  | return_flag    | boolean | Whether the transaction included a return | TRUE |
  | region_code    | string | Two-letter identifier for store region | "NE" |

  WHAT TO AVOID:
  ❌ Skipping this section because "the field names are self-explanatory."
     They're not. Not to a reviewer. Not to you in six months.

  📌 FOR SQL PROJECTS: If you have multiple tables, create one block per table.
     Describe join keys and relationships here. Your ERD (Section 7) will
     visualise what this section describes in text.

  📌 FOR NON-SQL PROJECTS: Describe the shape of your dataset informally
     if a formal schema doesn't apply. Even one paragraph is more helpful than nothing.
-->

### Dataset / Table: `[ccc_info]`

| Field Name | Data Type | Description | 
|------------|-----------|-------------|
| `[customer_id]` | [int] | [customers id] | 
| `[first_name]` | [varchar(50)] | [customers first name] | 
| `[last_name]` | [varchar(50)] | [customers last name] | 
| `[age]` | [int] | [customers age] | 
| `[credit_score]` | [int] | [customers credit score] | 
| `[anual_income]` | [decimal(8, 2)] | [customers annual income] |
| `[occupation]` | [varchar(50)] | [customers occupation] |


### Dataset / Table: `[ccc_balance]`

| Field Name | Data Type | Description | 
|------------|-----------|-------------|
| `[customer_id]` | [int] | [customers id] | 
| `[outstanding_balance]` | [decimal(8, 2)] | [customers outstanding balance] | 
| `[statement_balance]` | [decimal(8, 2)] | [customers statement balance] | 
| `[payment_amount]` | [decimal(8, 2)] | [customers payment amount] | 

### Dataset / Table: `[ccc_type]`

| Field Name | Data Type | Description | 
|------------|-----------|-------------|
| `[customer_id]` | [int] | [customers id] | 
| `[card_type]` | [varchar(50)] | [customers credit card company] |
| `[credit_limit]` | [int] | [customers credit limit] | 
| `[card_age]` | [int] | [how long the customer has had the credit card] |

### Dataset / Table: `[ccc_behavior]`

| Field Name | Data Type | Description | 
|------------|-----------|-------------|
| `[customer_id]` | [int] | [customers id] | 
| `[monthly_transactions]` | [int] | [customers monthly transactions] | 
| `[monthly_spending]` | [decimal(8,2)] | [customers monthly spending] | 
| `[online_shopping]` | [decimal(8,2)] | [customers online spending] | 
| `[grocery_spending]` | [decimal(8,2)] | [customers grocery spending] | 
| `[fuel_spending]` | [decimal(8,2)] | [customers fuel spending] | 
| `[dining_spending]` | [decimal(8,2)] | [customers dining spending] | 
| `[travel_spending]` | [decimal(8,2)] | [customers travel spending] | 
| `[entertainment_spending]` | [decimal(8,2)] | [customers entertainment spending] | 
| `[utility_spending]` | [decimal(8,2)] | [customers utility spending] | 

---


## 4. Analysis & Metrics
---
### Analytical Approach

[Describe how you approached the analysis. Were you exploring patterns? Testing a hypothesis? Building and validating a pipeline? Be honest about your method - exploratory work is valid, just call it that.]

### Key Metrics Defined

| Metric | Plain-Language Definition | Why It Matters |
|--------|--------------------------|----------------|
| `[Metric 1]` | [What it measures, in one sentence] | [What decision or question it answers] |
| `[Metric 2]` | [What it measures, in one sentence] | [What decision or question it answers] |
| `[Metric 3]` | [What it measures, in one sentence] | [What decision or question it answers] |

### Methods Used

- [e.g., Descriptive statistics - distribution, central tendency, outlier detection]
- [e.g., Trend analysis across [time period]]
- [e.g., Segmentation / group comparison by [dimension]]
- [e.g., Correlation analysis between [variable A] and [variable B]]
- [e.g., SQL window functions for [specific aggregation]]
- [e.g., Custom aggregation or transformation logic in [tool]]

---

## 5. Author

**[Juan Arredondo]**

- 🔗 [LinkedIn URL]
- 💼 [Portfolio or GitHub profile URL]
- 📧 [juanarrofficial@gmail.com]

---
