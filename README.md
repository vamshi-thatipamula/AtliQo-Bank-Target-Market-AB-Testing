# AtliQo Bank Credit Card Strategy: Target Market Analysis & A/B Testing

![Project Banner](assets/project_banner.png)

![Python](https://img.shields.io/badge/Python-3.x-blue)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-yellow)
![NumPy](https://img.shields.io/badge/NumPy-Numerical%20Computing-blue)
![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualization-orange)
![Seaborn](https://img.shields.io/badge/Seaborn-Statistical%20Plots-lightblue)
![Statsmodels](https://img.shields.io/badge/Statsmodels-Statistical%20Modeling-green)
![MySQL](https://img.shields.io/badge/MySQL-Database-blue)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange)
![A/B Testing](https://img.shields.io/badge/A%2FB%20Testing-Experimentation-red)

---

## 🚀 Project Overview

This project focuses on designing and validating a credit card strategy for AtliQo Bank using exploratory data analysis and A/B testing. The goal is to identify a high-potential customer segment and evaluate the effectiveness of a new credit card before a full-scale launch.

---

## 1. Business Problem

AtliQo Bank aims to launch a new credit card in the highly competitive Indian market, where established players already offer well-targeted products.

The key challenge is:

> Identifying the right customer segment and designing a credit card that drives high adoption and increases customer spending.

To address this, the bank needs a data-driven approach to:
- Identify an underserved but high-potential customer segment  
- Understand customer spending behavior and payment preferences  
- Validate whether the new credit card improves transaction value through controlled experimentation  

The goal is to ensure that the product is not only well-targeted but also statistically validated before a full-scale launch.

---

## 2. Project Overview

This project follows a data-driven approach to support the launch of a new credit card by AtliQo Bank.

The analysis is structured into two key phases:

- Phase 1: Find Target Market 
  - Analyze customer demographics, financial profiles, and transaction behavior to identify a high-potential and underserved segment.


- Phase 2: A/B testing for new Credit Card
  - Design and execute an experiment to evaluate whether the new credit card leads to a measurable improvement in customer spending compared to the existing card.

By combining exploratory data analysis with statistical testing, the project ensures that business decisions are:
- Insight-driven  
- Experimentally validated  
- Focused on measurable impact  

The final outcome is a clear recommendation on both the target segment and the effectiveness of the new credit card.

---

## 3. Project Objectives

The objective of this project is to support a data-driven credit card launch strategy for AtliQo Bank by combining customer analysis with experimental validation.

Key objectives include:

- Perform data cleaning and exploratory analysis to ensure data quality  
- Analyze customer demographics, financial profiles, and transaction behavior  
- Identify an underserved but high-potential target segment  
- Understand spending patterns across age groups, platforms, and product categories  
- Design and execute an A/B testing framework to evaluate the new credit card  
- Measure the impact of the new card on transaction behavior using statistical methods  
- Provide actionable recommendations based on both insights and experimental results  

The overall goal is to ensure that the credit card launch is targeted, validated, and backed by data-driven evidence.

---

## 4. Project Highlights

- End-to-end data science project covering both **exploratory analysis and experimental validation**  
- Identified an **untapped customer segment (18–25 age group)** with high growth potential  
- Performed extensive **data cleaning, feature engineering, and multi-table data integration**  
- Conducted in-depth **EDA on demographics, financial behavior, and transaction patterns**  
- Designed and executed an **A/B testing framework** to validate product effectiveness  
- Applied **statistical methods** including Z-test, p-value analysis, and effect size evaluation  
- Achieved a **~6.7% increase in transaction value** with the new credit card  
- Demonstrated both **statistical significance and practical business impact**  
- Delivered **actionable recommendations** for targeted credit card launch  

---

## 5. Dataset Information & Credit

The dataset used in this project was provided as part of the course **Math and Statistics**, conducted by **Codebasics**.

Full credit goes to the **Mr. Dhaval Patel** and the Codebasics team for providing the dataset and learning resources.

> **Note:** The dataset is not publicly available and is therefore not included in this GitHub repository due to sharing restrictions.

This project is created strictly for educational and portfolio demonstration purposes.

---

## 6. Database Structure

The project uses a **multi-table relational dataset**, organized across two phases. Each phase utilizes specific tables to support analysis and decision-making.

### 6.1 Phase 1: Find Target Market

Phase 1 focuses on understanding customer behavior, financial profiles, and transaction patterns using three core tables:

#### 6.1.1 Customers Table

Contains **demographic information** of customers.

**Columns:**

* `cust_id` – Unique customer identifier
* `name` – Customer name
* `gender` – Gender
* `age` – Age
* `location` – Geographic location
* `occupation` – Profession
* `annual_income` – Yearly income
* `marital_status` – Marital status

#### 6.1.2 Credit Profiles Table

Contains **credit-related and financial attributes**.

**Columns:**

* `cust_id` – Unique customer identifier used to link tables
* `credit_score` – Credit rating
* `credit_utilisation` – Credit usage ratio
* `outstanding_debt` – Current debt
* `credit_inquiries_last_6_months` – Recent credit checks
* `credit_limit` – Maximum credit available

#### 6.1.3 Transactions Table

Captures **transaction-level behavior and spending patterns**.

**Columns:**

* `tran_id` – Unique transaction identifier
* `cust_id` – Unique customer identifier used to link tables
* `tran_date` – Date of transaction
* `tran_amount` – Transaction value
* `platform` – Platform used
* `product_category` – Category of purchase
* `payment_type` – Mode of payment

### 6.2 Phase 2: A/B testing for new Credit Card

Phase 2 focuses on evaluating the performance of the new credit card using campaign data.

#### 6.2.1 Transactions After Campaign Table

Contains **aggregated transaction data** for control and test groups.

**Columns:**

* `campaign_date` – Date of observation
* `control_group_avg_tran` – Average transaction (control group)
* `test_group_avg_tran` – Average transaction (test group)

---

## 7. Tools and Technologies

The project utilizes a combination of tools for data analysis, visualization, database management, and statistical testing:

- **Python** – Core programming language
- **pandas, numpy** – Data cleaning, transformation, and analysis
- **matplotlib, seaborn** – Data visualization
- **scipy, statsmodels** – Statistical analysis and A/B testing
- **MySQL (MySQL Workbench)** – Data storage and querying
- **Jupyter Notebook (PyCharm)** – Development and experimentation environment

---

## 8. Project Workflow

The project follows a structured two-phase approach to ensure a data-driven and experimentally validated credit card launch strategy.

- Phase 1: Find Target Market focuses on analyzing customer demographics, financial attributes, and transaction behavior to identify a suitable target segment
- Phase 2: A/B testing for new Credit Card focuses on designing and executing an experiment to evaluate the effectiveness of the new credit card

### 8.1 Phase 1: Find Target Market

This phase involves a comprehensive analysis of customer, credit, and transaction data to understand behavioral patterns and identify a high-potential customer segment.

#### 8.1.1 Customer Table Analysis

**Annual Income Analysis**

The analysis began with evaluating the annual income column, as it is a key indicator of customer purchasing power and financial capability.

- Performed initial data validation to identify missing values and inconsistencies
- Handled missing values using occupation-wise median imputation, ensuring that replacements reflect realistic income patterns across professions
- Identified outliers using statistical methods and validated them against business constraints
- Conducted distribution analysis to understand:
  - Income spread 
  - Skewness 
  - Presence of extreme values

![Distribution of Annual Income](Phase1_Find_Target_Market/data_visualization/distribution_of_annual_income.png)

- Performed group-level comparisons to analyze how income varies across:
  - Occupation 
  - Gender 
  - Location 
  - Marital status

![Average Annual Income by Demographics](Phase1_Find_Target_Market/data_visualization/average_annual_income_by_demographics.png)

**Age Analysis**

Age was analyzed to enable meaningful customer segmentation and behavioral comparison.

- Verified that the column contains no missing values
- Identified unrealistic values (e.g., age below minimum working age or above realistic limits)
- Treated outliers using occupation-based median replacement to maintain consistency

![Customer Age Distribution](Phase1_Find_Target_Market/data_visualization/customer_age_distribution.png)

- Created a new feature: age groups
  - 18–25 
  - 26–48 
  - 49–65
- Analyzed distribution of customers across these groups

![Distribution of Age Groups](Phase1_Find_Target_Market/data_visualization/distribution_of_age_groups.png)

- Evaluated demographic distribution across gender and location

![Customer Distribution by Location and Gender](Phase1_Find_Target_Market/data_visualization/customer_distribution_by_location_and_gender.png)

#### 8.1.2 Credit Profile Analysis

This step focused on understanding customer creditworthiness and financial strength.

- Identified and removed duplicate records to ensure data consistency
- Analyzed the credit_limit column and handled missing values using a credit score-based grouping approach, where values were imputed using the most representative value within each group

![Credit Score vs Credit Limit](Phase1_Find_Target_Market/data_visualization/credit_score_vs_credit_limit.png)

- Detected invalid scenarios where:
  - outstanding_debt exceeded credit_limit
- Applied business rules to correct these inconsistencies

![Outstanding Debt Box Plot](Phase1_Find_Target_Market/data_visualization/box_plot_for_outstanding_debt.png)

- Conducted correlation analysis across financial variables to understand relationships between:
  - Credit score 
  - Credit limit 
  - Credit utilization 
  - Debt levels

![Correlation Matrix](Phase1_Find_Target_Market/data_visualization/correlation_matrix.png)

- Explored the relationship between annual income and credit score to assess whether income is a strong predictor of creditworthiness

![Annual Income vs Credit Score](Phase1_Find_Target_Market/data_visualization/annual_income_vs_credit_score.png)

#### 8.1.3 Transaction Table Analysis

This step focused on analyzing customer spending behavior, payment preferences, and transaction patterns using transaction-level data.

**Data Cleaning**
- Handled missing values in the platform column using the most frequent category to maintain consistency
- Identified zero-value transactions and replaced them using median values within similar transaction groups to preserve realistic behavior
- Detected outliers in transaction amounts using the Interquartile Range (IQR) method

![Transaction Amount Before Cleaning](Phase1_Find_Target_Market/data_visualization/transaction_amount.png)

- Replaced extreme values using category-level aggregates to ensure meaningful and stable transaction values

![Transaction Amount After Cleaning](Phase1_Find_Target_Market/data_visualization/transaction_amount_cleaned.png)

**Behavioral Analysis**
- Analyzed the overall distribution of payment types to understand customer payment preferences

![Payment Types Distribution](Phase1_Find_Target_Market/data_visualization/payment_types.png)

- Examined customer behavior across:
  - Product categories 
  - Platforms
  - Payment methods

![Platform Usage Across Product Categories](Phase1_Find_Target_Market/data_visualization/platform_usage_across_product_categories.png)

![Product Category and Platform Count Across Age Groups](Phase1_Find_Target_Market/data_visualization/product_category_and_platform_count_across_age_groups.png)

- Analyzed payment behavior across different age groups

![Payment Type Distribution Across Age Groups](Phase1_Find_Target_Market/data_visualization/payment_type_distribution_across_age_groups.png)

- Evaluated average transaction amounts across:
  - Payment types 
  - Platforms 
  - Product categories 
  - Customer segments

![Average Transaction Amount by Customer Segments](Phase1_Find_Target_Market/data_visualization/average_transaction_amount_by_customer_segments.png)

**Age Group Analysis**
- Performed comparative analysis across different age groups to understand variations in:
  - Financial attributes 
  - Credit behavior 
  - Transaction patterns
- Combined multiple dimensions of analysis to build a comprehensive behavioral profile for each segment

![Average Financial Metrics by Age Group](Phase1_Find_Target_Market/data_visualization/average_financial_metrics_by_age_group.png)

#### 8.1.4 Target Market Identification

- Integrated insights from customer demographics, credit profiles, and transaction behavior
- Conducted comparative analysis across segments to identify differences in:
  - Financial capability 
  - Credit readiness 
  - Spending behavior
- Evaluated potential target segments based on:
  - Customer distribution 
  - Behavioral patterns 
  - Financial characteristics
<br>

**Target Segment Evidence (18–25 Age Group)**

<table>
<tr>
<td>
<img src="Phase1_Find_Target_Market/data_visualization/distribution_of_age_groups.png" width="100%"/><br>
<sub><b>~25% of customers fall in 18–25 age group</b></sub>
</td>

<td>
<img src="Phase1_Find_Target_Market/data_visualization/average_annual_income_by_demographics.png" width="100%"/><br>
<sub><b>Lower average income compared to other segments</b></sub>
</td>

<td>
<img src="Phase1_Find_Target_Market/data_visualization/average_financial_metrics_by_age_group.png" width="100%"/><br>
<sub><b>Limited credit history (low score & limit)</b></sub>
</td>
</tr>

<tr>
<td>
<img src="Phase1_Find_Target_Market/data_visualization/payment_type_distribution_across_age_groups.png" width="100%"/><br>
<sub><b>Low credit card usage across this segment</b></sub>
</td>

<td>
<img src="Phase1_Find_Target_Market/data_visualization/average_transaction_amount_by_customer_segments.png" width="100%"/><br>
<sub><b>Lower transaction value vs other groups</b></sub>
</td>

<td>
<img src="Phase1_Find_Target_Market/data_visualization/product_category_and_platform_count_across_age_groups.png" width="100%"/><br>
<sub><b>High engagement in Electronics, Fashion & Beauty</b></sub>
</td>
</tr>
</table>

#### 🎯 Final Target Segment Decision

> **The 18–25 age group represents a high-potential, underpenetrated segment with strong digital engagement but low credit card adoption.**
>
> Despite having lower income and limited credit history, this segment shows consistent transaction activity and clear product preferences, making it an ideal candidate for a tailored, entry-level credit card offering.
>
> The analysis strongly supports targeting this segment for the initial credit card launch to maximize adoption and long-term customer value.

### 8.2 Phase 2: A/B testing for new Credit Card

This phase focuses on validating the effectiveness of the new credit card using a structured experimental approach.

#### 8.2.1 Pre-Campaign (Campaign Planning)

- Determined required sample size using:
  - Effect size 
  - Statistical power
- Evaluated multiple sample size scenarios based on business constraints and feasibility
- Selected an appropriate sample size for the experiment
- Defined experimental groups:
  - Test group → New credit card 
  - Control group → Existing credit card

#### 8.2.2 Execute Campaign (Support Campaign Launch)

- Deployed the new credit card to the selected test group
- Assigned the existing credit card to the control group
- Executed the campaign over a defined time period
- Monitored customer transaction behavior throughout the campaign duration

#### 8.2.3 Post-Campaign Data Collection

- Collected transaction data for both control and test groups
- Aggregated the data to compute average transaction metrics

![Average Transaction Amounts in Both Groups](Phase2_A_B_Testing_for_New_Credit_Card/data_visualization/Average_transaction_amounts_in_both_groups.png)

![A/B Test Distribution](Phase2_A_B_Testing_for_New_Credit_Card/data_visualization/AB_test_distribution_of_average_transaction_amounts.png)
- Prepared the dataset for statistical analysis

#### 8.2.4 Hypothesis Testing & Evaluation

- Defined null and alternative hypotheses to compare the performance of the two groups
- Performed Two-Sample Z-test to evaluate differences in average transaction values
- Interpreted results using:
  - Critical value (rejection region)
  - p-value approach 
  - statsmodels implementation
- Calculated additional metrics such as:
  - Uplift in performance 
  - Effect size to assess practical significance
- Conducted a robustness check using t-test to validate consistency of results

---

## 9. Key Insights

### 9.1 Customer Segmentation & Demographics
- The 18–25 age group accounts for ~25% of the customer base, making it a significant segment for targeted strategies
- This segment has lower average income (<50K), indicating early-stage earning potential compared to older groups

### 9.2 Credit Behavior Insights
- Customers in the 18–25 segment have limited credit history, reflected in lower credit scores and credit limits
- A strong relationship exists between credit score and credit limit, indicating creditworthiness is behavior-driven
- Annual income shows no strong relationship with credit score, suggesting income alone is not a reliable predictor of credit eligibility

### 9.3 Transaction & Payment Behavior
- The 18–25 segment shows low credit card usage despite being highly active in digital transactions
- Customers in this group frequently spend on:
  - Electronics 
  - Fashion & Apparel 
  - Beauty & Personal Care
- Payment behavior is dominated by digital methods (UPI, online payments) rather than credit cards

### 9.4 Behavioral Gap Identified
- There is a clear gap where customers are:
  - Digitally active and spending regularly 
  - But underutilizing credit cards

- This highlights a strong opportunity for targeted credit card offerings

### 9.5 A/B Testing Insights
- The test group using the new credit card shows a higher average transaction value compared to the control group
- The improvement is statistically significant (p-value < 0.05), confirming that the difference is not due to random variation
- The observed uplift of ~6.7% indicates a meaningful improvement in customer spending behavior
- The effect size (~0.49) suggests a moderate and practically significant impact

---

## 10. Key Takeaways

- The 18–25 age group is the most suitable target segment, offering strong growth potential despite current low credit card adoption
- There is a clear opportunity to design a digital-first credit card aligned with online spending behavior and popular product categories
- Credit card targeting should focus more on behavioral indicators (credit score, usage patterns) rather than income alone
- The new credit card has been successfully validated through A/B testing, reducing uncertainty before large-scale deployment
- The observed increase in transaction value indicates that the product can drive higher customer engagement and revenue potential
- A combination of EDA-driven segmentation and experimental validation provides a robust framework for making reliable business decisions

---

## 11. Skills Demonstrated

- **Data Cleaning & Preprocessing** – Handling missing values, outlier treatment (IQR, business rules)
- **Exploratory Data Analysis (EDA)** – Analyzing customer, financial, and transaction data
- **Feature Engineering** – Creating age groups and credit score segments
- **Data Integration** – Merging multiple tables for unified analysis
- **Statistical Analysis** – Hypothesis testing (Z-test), p-value, confidence intervals
- **A/B Testing** – Experiment design, sample size calculation, test vs control evaluation
- **Data Visualization** – Building charts to analyze distributions and patterns
- **Business Problem Solving** – Identifying target segment and validating product strategy

---

## 12. Project Structure (Folder structure + Data Flow)

The project is organized into two phases, reflecting the complete workflow from target market identification to experimental validation.

### 12.1 Folder Structure

```
AtliQo-Bank-Project/
│
├── Phase1_Find_Target_Market/
│   ├── phase_1_find_target_market.ipynb
│   └── data_visualization/
│
├── Phase2_A_B_Testing_for_New_Credit_Card/
│   ├── phase_2_A_B_testing_for_new_credit_card.ipynb
│   └── data_visualization/
│
├── assets/
│   └── project_banner.png
│
├── README.md
├── requirements.txt
├── .gitignore
```

### 12.2 Data Flow

```
Data Sources (Customers, Credit Profiles, Transactions)
        ↓
Data Cleaning & Preprocessing
        ↓
Data Integration (Merge using cust_id)
        ↓
Phase 1: Find Target Market
        ↓
EDA & Segmentation
        ↓
Target Market Identified
        ↓
Phase 2: A/B Testing
        ↓
Experiment Design → Campaign Execution
        ↓
Post-Campaign Data Collection
        ↓
Hypothesis Testing & Evaluation
        ↓
Final Decision
```

---

## 13. Project Architecture

```
┌──────────────────────────┐     ┌──────────────────────────┐     ┌──────────────────────────┐     ┌──────────────────────────┐     ┌──────────────────────────┐
│      Data Sources        │     │ Data Processing Layer    │     │      Analysis Layer      │     │    Statistical Layer     │     │     Business Output      │
│--------------------------│     │--------------------------│     │--------------------------│     │--------------------------│     │--------------------------│
│ Customers Table          │     │ Data Cleaning            │     │ Phase 1: Find Target     │     │ Hypothesis Testing       │     │ Target Segment Identified│
│ Credit Profiles Table    │     │ Data Transformation      │     │ Market (EDA & Segmentation)│   │ Z-test, p-value          │     │ Credit Card Validation   │
│ Transactions Table       │     │ Data Integration         │     │ Phase 2: A/B Testing     │     │ Effect Size              │     │ Final Decision           │
│ (CSV Files, MySQL DB)    │     │ (Merge using cust_id)    │     │                          │     │                          │     │                          │
└──────────────┬───────────┘     └──────────────┬───────────┘     └──────────────┬───────────┘     └──────────────┬───────────┘     └──────────────┬───────────┘
               │                                │                                │                                │                                │
               └──────────────►─────────────────┴──────────────►─────────────────┴──────────────►─────────────────┴──────────────►─────────────────┘
```

---

## 14. How to run the project

### 14.1 Install dependencies:


    pip install -r requirements.txt

### 14.2 Run notebooks:

    Phase1_Find_Target_Market/phase_1_find_target_market.ipynb
    Phase2_A_B_Testing_for_New_Credit_Card/phase_2_A_B_testing_for_new_credit_card.ipynb

---

## 15. Final Conclusion

1. The project demonstrates a complete **data-driven approach to product strategy**, starting from customer analysis to experimental validation.
2. By identifying the **18–25 age group as a high-potential segment** and validating the new credit card through **A/B testing**, the analysis provides strong evidence for a targeted and low-risk product launch.
3. The combination of **exploratory data analysis and statistical testing** ensures that decisions are not only insight-driven but also **quantitatively validated**, improving confidence in business outcomes.
4. Overall, this project highlights the importance of **aligning customer behavior with product design and validating decisions through experimentation** to drive effective and scalable business strategies.








