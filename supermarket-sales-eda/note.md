# Analysis Notes

## Method

I first checked the dataset structure, data types, missing values and duplicate rows.

The dataset contains 1,000 transactions and 17 columns, with no missing values found.

The `Date` and `Time` columns were converted into proper formats before the time-based analysis. I also extracted the hour from the `Time` column and created a month field from `Date`.

For the main analysis, I compared both total sales and order count across:

- Branch
- Product line
- Customer type
- Gender

I used both measures because a category with more transactions does not always generate more revenue.

## Key Findings

### Product lines

Food and Beverages generated the highest revenue at around **$56.1K**.

Health and Beauty had the lowest total revenue at approximately **$49.2K**.

The difference between the product lines was not very large, so sales were relatively well distributed across categories instead of depending heavily on one product group.

### Branches

Branch C recorded the highest overall revenue at about **$110.6K**.

Interestingly, Branch A had more transactions, but Branch C still generated more sales. This suggests that the average order value was higher in Branch C.

### Customer types

The customer split was almost equal:

- Member customers: **50.1%**
- Normal customers: **49.9%**

There was no major difference in transaction volume between the two groups.

### Time patterns

The busiest hour was **19:00**, which was also one of the strongest periods in terms of sales.

Another clear increase appeared around **13:00**.

This shows that customer activity is concentrated mainly around lunch and evening hours.

January had the highest monthly sales, reaching roughly **$116K**.

## Business Insights

1. **Food and Beverages is the strongest product line**, but the difference between the highest and lowest performing categories is still fairly small. Revenue is therefore spread across several product groups rather than depending on one category.

2. **Branch C generates the most revenue despite not having the highest number of transactions.** This may indicate stronger average basket value or higher-value purchases at that branch.

3. **Member and Normal customers behave very similarly in terms of order volume.** Since membership does not create a clear difference in visit frequency, it would be useful to compare spending per order between the two groups.

4. **19:00 is the busiest hour, with another visible peak around 13:00.** These periods would be the most relevant for staff scheduling, checkout capacity and time-based promotions.

5. **January generated the highest revenue in the available period.** However, because the dataset covers only a short timeframe, this should not be treated as a long-term seasonal trend without more historical data.

## Final Note

The strongest differences in this dataset came from branch performance, product category revenue and time of day.

One useful takeaway was that transaction count alone does not explain performance. Branch C is a good example: it did not lead in order count, but it still produced the highest revenue.