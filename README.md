
# Sales Strategy Evaluation for New Product Line – Pens and Printers

This data analytics project was conducted as part of the DataCamp Data Analyst Professional Certification. The analysis explores the performance of different sales strategies used by Pens and Printers to sell a newly launched line of office stationery.

## Project Background

Pens and Printers, founded in 1984, supplies high-quality office products to large organizations. While the company does not manufacture its own goods, it is a trusted reseller for a wide range of essentials.

Recently, the company launched a new product line focused on brainstorming tools like notebooks and sticky notes. To determine the best method to promote these products, three sales strategies were tested:

- Email only
- Phone call only
- Email followed by a phone call

This project evaluates the effectiveness of each approach based on revenue generation and customer response.

## Business Questions

The sales team requested insights into the following:

- Number of customers per sales approach
- Overall and per-method revenue distribution
- Revenue trends over time by method
- Recommended strategy based on effort vs. performance
- Additional contextual differences between customer groups

## Data Structure and Cleaning

The dataset includes one record per customer and the following columns:

| Column | Description |
|--------|-------------|
| week | Week of sale since product launch |
| sales_method | Sales method used (email, call, both) |
| customer_id | Unique customer identifier |
| nb_sold | Number of products sold |
| revenue | Revenue from this customer |
| years_as_customer | Customer tenure |
| nb_site_visits | Website visits in the last 6 months |
| state | Customer location |

### Data Validation and Cleaning Steps

- Checked for and addressed missing values
- Ensured consistent categorical values (e.g., "email", "call", "both")
- Verified appropriate value ranges and data types
- Detected and reviewed outliers in revenue

## Exploratory Data Analysis

### Key Insights

- The "Email + Call" method yielded the highest average revenue per customer.
- Customers with higher site visit frequency tended to generate more revenue.
- Week 3–4 saw the highest revenue across all methods, with the "Email + Call" method sustaining performance longer.
- The "Email" method reached the most customers but had the lowest average revenue.

Visualizations and analysis are included in the notebook: `Final Project Notebook.ipynb`

## Metric Definition

To support ongoing evaluation, the recommended metric is:

**Average Weekly Revenue per Sales Method**

This balances efficiency and outcome. Example values:

| Method | Average Weekly Revenue |
|--------|-------------------------|
| Email | $XX.XX |
| Call | $XX.XX |
| Email + Call | $XX.XX |

(Insert specific values from the analysis)

## Executive Summary

The dual-contact "Email + Call" strategy achieved the highest returns but also required more effort. For a scalable approach, the "Call-only" method provides solid performance with less resource demand. "Email-only" should be reserved for broad outreach where cost is a constraint.

## Insights Deep Dive

### Revenue by Method

- Email + Call: High revenue, fewer customers
- Call: Moderate revenue and effort
- Email: Most customers, least revenue

### Revenue Over Time

- Revenue peaked during weeks 3–4
- Dual contact method sustained performance beyond the peak

### Customer Characteristics

- Tenure and site engagement showed minor but consistent correlation with revenue

### Revenue Distribution

- All methods showed right-skewed revenue distribution, with the Email method showing the most variance

## Recommendations

- Prioritize the "Email + Call" strategy for high-value or long-tenure customers
- Use "Call-only" when balancing performance with resource constraints
- Use "Email-only" for low-effort mass outreach
- Implement ongoing monitoring of average revenue per method
- Consider segmentation for targeted strategy deployment

## Assumptions and Caveats

- Revenue assumed to represent success; time-cost data was unavailable
- Analysis is limited to a single product line over a six-week period
- Some external factors (e.g., product mix) were not captured in the dataset

## Project Files

- Jupyter Notebook: `Final Project Notebook.ipynb`
- Case Study PDF: `Case Study (1).pdf`
