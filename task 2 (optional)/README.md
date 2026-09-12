# Supermarket Sales EDA

A short exploratory analysis of supermarket transaction data, focused on how sales vary across branches, product lines, customer groups and different hours of the day.

The aim was not just to calculate totals, but to compare the main business segments and see where sales activity was actually concentrated.

## What I looked at

- Revenue and order count by branch
- Product line performance
- Customer type and gender distribution
- Hourly sales activity
- Strongest and weakest product categories
- Sales differences between branches and product lines

## Dataset

The dataset contains 1,000 supermarket transactions and 17 columns, including:

- Branch
- Customer type
- Gender
- Product line
- Unit price
- Quantity
- Total
- Date and Time
- Gross income
- Rating

No missing values were found in the dataset.

Source:  
[Supermarket Sales Dataset](https://github.com/cwentz12/Supermarket-Sales-Analysis/blob/main/Data/supermarket_sales%20-%20Sheet1.csv)

## Tools

- Python
- pandas
- matplotlib
- seaborn
- Jupyter Notebook

## Main findings

Food and Beverages generated the highest total revenue at roughly **$56.1K**, while Health and Beauty recorded the lowest at about **$49.2K**.

Branch C produced the highest overall sales, reaching around **$110.6K**, even though its number of transactions was not the highest.

Customer activity was almost evenly divided between the two customer groups: **Members accounted for 50.1% of orders and Normal customers for 49.9%**.

Sales activity was strongest around **19:00**, with another visible peak around **13:00**. This suggests that lunch and evening hours are the most active periods of the day.

## Visual analysis

The notebook includes four visualizations:

- Product line revenue ranking
- Customer type order share
- Hourly sales trend
- Branch × Product line sales heatmap

Together, they provide a quick view of which categories, branches and time periods contribute most to supermarket sales.

## Project files

- `supermarket_sales_basic_eda.ipynb` — full analysis and visualizations
- `supermarket_sales - Sheet1.csv` — source dataset
- `note.md` — methodology and key observations