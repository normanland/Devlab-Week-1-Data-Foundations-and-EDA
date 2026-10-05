# Notes about analysis

## Used Methodology

I started with a quick quality check for missing values, duplicates and column types. The dataset contains 99,457 transactions and 10 original columns, with no missing values.

The `invoice_date` field was converted to datetime and used to create year, month and monthly period fields.

For revenue, I used the existing `price` column directly. In this dataset, the price already reflects the amount paid for the selected quantity, so multiplying it by `quantity` again would overstate revenue.

The analysis was built around four dimensions:

- category
- shopping mall
- payment method
- gender

I also used pivot tables to compare mall and category revenue, yearly category trends, and gender spending patterns. Two extra checks were added for month-over-month mall growth and the leading payment method in each category.

## Business Insights

1. **Clothing carries the largest share of the business.** It generates about **45% of total revenue** and records more than **103K units sold**. AVM management should keep strong stock availability and visibility for this category, especially in the highest-volume malls, but should also watch the risk of depending too heavily on one product group.

2. **Mall of Istanbul and Kanyon are the two strongest locations by total revenue**, contributing roughly **40% combined**. These malls are good places to test new promotions first because they provide the largest revenue base. On the other hand, **Emaar Square Mall has the highest average purchase value**, so increasing traffic there may have more impact than trying to push basket size higher.

3. **Female customers contribute close to 60% of revenue**, and the same pattern appears across all major categories. Average purchase value is almost identical between women and men, which means the revenue gap is mainly explained by transaction volume rather than larger baskets. Retaining female traffic remains important, while male visit frequency is a clear growth opportunity.

4. **Cash is the dominant payment method in every category**, usually accounting for roughly **44–46% of transactions**. Credit cards still represent around one-third of purchases, so card-based offers could be tested in higher-value categories such as Technology and Shoes without changing the overall payment mix too aggressively.

5. **2022 revenue is only slightly higher than 2021, while 2023 is a partial year ending in early March.** The lower 2023 total should not be treated as evidence of a decline. Month-over-month growth also moves sharply across malls, so future management reporting should compare the same months year over year before making performance decisions.

## Final Note

The strongest pattern is revenue concentration: Clothing, Shoes and Technology together generate the vast majority of sales value, while Mall of Istanbul and Kanyon lead by total revenue.

At the same time, customer spending per transaction is fairly balanced by gender, and payment preferences are consistent across categories. This makes location traffic, category mix and stock planning more important management levers than broad demographic differences alone.
