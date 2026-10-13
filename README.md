# Harbour & Co. — E-commerce Profitability & Performance Analysis

## Project Overview

Harbour & Co. is an e-commerce business case study focused on understanding how effectively revenue is converted into profit.

This project analyses sales transactions, product information, customer segments, and marketing campaigns to evaluate business performance across sales channels, products, customer groups, geographic markets, and promotional activities.

Rather than focusing solely on revenue growth, the analysis investigates the underlying drivers of profitability and identifies opportunities to support more sustainable, profit-oriented growth.

**Core business question:** How can Harbour & Co. improve profitability and make better commercial decisions using data-driven insights?

## Business Context

Harbour & Co. generates substantial revenue across three sales channels: Website, Amazon, and eBay. However, strong sales performance does not necessarily translate into equally strong profitability.

The analysis focuses on several key business questions:

- Which sales channels generate the most revenue and gross profit?
- Which products and categories contribute most to profitability?
- How do discounts and marketing campaigns relate to profit margins?
- Which customer segments and geographic markets offer the strongest opportunities?
- How significant are product returns to overall business performance?
- Where should management prioritise improvements to achieve more profitable growth?

## Analytical Approach

The project follows an end-to-end analytical workflow, from data quality assessment to business recommendations.

### 1. Data Discovery & Quality Assessment

- Inspected dataset dimensions, column structures, data types, and missing values.
- Checked duplicate records, unique identifiers, categorical inconsistencies, and suspicious numerical values.
- Examined relationships between sales transactions, products, customers, and campaigns.
- Investigated date inconsistencies, negative quantities, and extreme transaction quantities.

### 2. Data Cleaning & Preparation

- Removed 18 exact duplicate records from the sales transactions dataset.
- Standardised categorical values, including customer segments and product categories.
- Resolved a duplicate customer master record.
- Imputed 65 missing shipping cost values using median shipping costs grouped by state and sales channel.
- Parsed inconsistent order dates and removed two records with dates that could not be recovered.
- Preserved negative quantities for return-related analysis rather than automatically converting them to positive values.
- Retained transactions with missing customer identifiers to avoid unnecessary loss of valid sales records.
- Validated cleaned datasets before conducting further analysis.

### 3. Exploratory Data Analysis (EDA)

Analysed business performance across six major dimensions:

| Analytical area | Focus |
|---|---|
| Overall performance | Revenue, gross profit, profit margin, and transaction trends |
| Sales channels | Comparative performance across Website, Amazon, and eBay |
| Products & categories | Revenue contribution, gross profit, and margin differences |
| Customers | Revenue and profitability by customer segment |
| Geography | State-level revenue concentration and profitability |
| Discounts, campaigns & returns | Promotional performance, margin trade-offs, and return rates |

Additional cross-analysis examined the interaction between sales channels, product categories, customer segments, discount levels, and individual products.

### 4. Business Insights & Recommendations

Translated analytical findings into actionable recommendations focused on channel profitability, promotional efficiency, product mix, and ongoing performance monitoring.

## Key Findings

### 1. A stable revenue base with limited evidence of organic growth

Harbour & Co. generated approximately **$13.55 million in net revenue** and **$4.90 million in gross profit** across 49,995 transactions, with an overall gross profit margin of approximately 36.15%.

Monthly revenue and profitability remained relatively stable throughout the two-year observation period, with no clear sustained upward trend.

**Business implication:** Future growth opportunities should focus on improving the profitability of existing operations rather than relying solely on increasing sales volume.

### 2. The Website generates the most revenue but has lower profitability

| Sales channel | Net revenue | Gross profit margin |
|---|---:|---:|
| Website | $6.73M | 35.63% |
| eBay | $3.44M | 36.70% |
| Amazon | $3.38M | 36.63% |

The Website is the largest revenue channel but consistently records lower profit margins than Amazon and eBay across the product categories and customer segments analysed.

**Business implication:** Investigate shipping costs, discounting, product mix, and channel-specific pricing practices to identify opportunities to improve Website profitability.

### 3. Higher discounts and campaign activity are associated with lower margins

| Discount level | Gross profit margin |
|---|---:|
| No discount | 37.81% |
| 1–5% | 35.21% |
| 6–10% | 31.07% |
| 11–20% | 25.69% |

Transactions associated with campaigns achieved a gross profit margin of 28.76%, compared with 37.40% for transactions without campaigns.

These results show a strong association between discount intensity and lower margins. However, the differences do not establish that campaigns themselves cause lower profitability, as product mix, sales channels, and other factors may also contribute.

**Business implication:** Evaluate promotions based on incremental profitable growth, not revenue or transaction volume alone.

### 4. Product mix creates opportunities to improve profitability

Smart Planner 09 was the strongest product by scale, generating approximately $574.7K in revenue and $217.3K in gross profit.

Meanwhile, Modern Storage Box 09 generated approximately $233.1K in revenue and $113.7K in gross profit, with a gross profit margin of approximately 48.75%.

At the category level, Technology Accessories recorded a lower gross profit margin of 32.99%, compared with 37.58% for Storage & Organisation.

**Business implication:** Distinguish between products that generate high absolute gross profit and those that generate stronger margins. Prioritise attractive product–channel combinations while reviewing the pricing, sourcing, and promotional strategies of lower-margin categories.

### 5. Geographic concentration creates both opportunities and risks

New South Wales, Victoria, and Queensland collectively account for approximately 80% of revenue.

Victoria generated approximately $3.67M in revenue and recorded a gross profit margin of 37.63%, while Western Australia generated approximately $1.27M in revenue with a margin of 32.48%.

**Business implication:** Protect and expand strong core markets while investigating the factors contributing to lower profitability in selected states.

### 6. Customer segments differ more in scale than in profitability

Individual customers generated approximately $5.80M in revenue and $2.10M in gross profit, making them the largest customer segment by scale.

However, gross profit margins across the four identified customer segments were relatively similar, ranging from approximately 36.07% to 36.22%.

**Business implication:** Customer segment alone may not be a major profitability differentiator. Combining segment analysis with channel, product, and promotional performance provides a more useful basis for commercial decisions.

### Supporting finding: Returns are not a major business-wide constraint

The overall return rate was approximately 1.81%, with relatively small differences across sales channels and product categories.

**Business implication:** Based on transaction frequency, improving channel profitability, discount efficiency, and product mix appears to be a higher priority than broad return-reduction initiatives.

## Business Recommendations

Based on the findings, four recommendations were developed:

**1. Improve Website Profitability**
- Investigate low-margin products and high shipping or discount costs.
- Compare product–channel profitability to identify opportunities for improvement.
- Monitor the margin gap between the Website and other sales channels.

**2. Introduce Discount Guardrails**
- Establish guidelines for routine promotional discounts.
- Require deeper discounts to be justified by expected incremental sales and profit.
- Track revenue, gross profit, and margin for each campaign.

**3. Prioritise High-Margin Products**
- Evaluate products using both gross profit contribution and profit margin.
- Identify opportunities to promote high-margin products such as Modern Storage Box 09.
- Review pricing, supplier costs, and product mix in lower-margin categories.

**4. Develop a Profitability Monitoring Dashboard**
- Prepare cleaned datasets for Power BI.
- Monitor revenue, gross profit, profit margin, sales channels, products, customer segments, geography, and discounts.
- Enable management to investigate changes in profitability through interactive filters and performance indicators.

The dashboard is a proposed next step supported by the analysis and recommendations; it should not be interpreted as a completed deliverable unless the Power BI dashboard is included in the repository.

## Tools & Technologies

- **Python** — Data analysis and preparation
- **Pandas** — Data cleaning, transformation, merging, and aggregation
- **Matplotlib** — Data visualisation and exploratory analysis
- **Jupyter Notebook / Google Colab** — Analytical workflow and documentation
- **Excel and CSV** — Source data formats
- **Power BI** — Intended next step for interactive profitability reporting

## Repository Structure

```text
Harbour-Co-Analysis/
├── README.md
├── Harbour_&_Co_Analysis.ipynb
├── data/
│   ├── 01_Sales_Transactions.csv
│   ├── 02_Product_Master.xlsx
│   ├── 03_Customer_Master.xlsx
│   └── 04_Campaign_Data.csv
└── outputs/
    ├── sales_clean.csv
    ├── products_clean.csv
    ├── customers_clean.csv
    └── campaigns_clean.csv
```

*The structure above is a suggested repository layout. Include only files that are actually present in your GitHub repository.*

## How to Run the Analysis

### Prerequisites

- Python 3.10 or later recommended
- Jupyter Notebook or Google Colab
- Required Python packages: `pandas`, `matplotlib`, `openpyxl`

### Setup

1. Clone or download the repository.
2. Install the required packages:

   ```bash
   pip install pandas matplotlib openpyxl
   ```

3. Place the four source datasets in the expected data directory, or update the file paths in the notebook.
4. Open `Harbour_&_Co_Analysis.ipynb` in Jupyter Notebook or Google Colab.
5. Execute the cells in order to reproduce the data quality checks, cleaning steps, exploratory analysis, and business insights.

The notebook currently references local files and a Google Drive directory in different sections. Update these paths to match your repository structure before running it outside the original environment.

## Project Outcomes

This project demonstrates an end-to-end business analytics approach through:

- Structured data quality assessment and cleaning.
- Multi-dimensional exploratory data analysis.
- Profitability analysis beyond headline revenue figures.
- Cross-analysis of channels, products, customers, geography, and promotions.
- Evidence-based business insights and prioritised recommendations.
- Preparation of cleaned datasets for downstream dashboard development.

## Conclusion

The analysis suggests that Harbour & Co.'s primary opportunity is not simply to generate more sales, but to convert its existing revenue base into more profitable growth.

By investigating Website margin performance, improving promotional discipline, prioritising attractive product–channel combinations, and establishing consistent profitability monitoring, the business can make more informed commercial decisions.

This project demonstrates how data analysis can bridge the gap between raw transactional data and practical business recommendations.

---

*This repository presents a business analytics case study. Findings and recommendations are based on the datasets and assumptions used in the accompanying notebook.*
