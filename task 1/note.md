# Hotel Booking Data Insights

## Dataset Note

The original task suggested using the sales_data_sample.csv retail dataset. For this project, I chose to work with the Hotel Booking Demand dataset instead.

The alternative dataset was selected to apply the same required data loading, cleaning, summary statistics and first-exploration techniques to a different business context. The core task requirements were preserved while the analysis was adapted to hotel booking behavior, cancellations, market segments and reservation patterns.

## Data Cleaning Notes

The dataset contains 119,390 hotel booking records and 32 columns.

During the cleaning process:

* `reservation_status_date` was converted from object to datetime format.
* Missing values were reviewed before applying any replacements.
* Missing `children` values were filled with `0`.
* Missing `country` values were labeled as `Unknown` because the original country could not be reliably inferred.
* Missing `agent` and `company` values were filled with `0` to represent records where no corresponding identifier was available.
* Duplicate rows were identified but not automatically removed. Since the dataset does not include a unique booking ID, identical rows may represent separate reservations with the same characteristics.
* `total_nights` was created by combining weekday and weekend stays.
* `total_guests` was created using adults, children and babies.
* Lead times were grouped into ranges to make cancellation patterns easier to compare.

After cleaning, the dataset was used for summary statistics and exploratory analysis.

## Initial Business Insights

1. **Cancellation is a major part of booking activity.**
   Around 37% of reservations were canceled. City Hotel showed a noticeably higher cancellation rate than Resort Hotel, approximately 41.7% compared with 27.8%. This suggests that City Hotel bookings may create greater uncertainty for occupancy planning.

2. **Online Travel Agencies are the dominant booking channel.**
   Online TA accounts for roughly 47% of all reservations. This makes online travel agencies an important source of demand, but also means their cancellation behavior can have a significant impact on overall hotel performance.

3. **Lead time is relevant when evaluating booking stability.**
   Reservations were made around 104 days in advance on average. Cancellation behavior varied across different lead-time groups, showing that how early a reservation is made can be useful when assessing cancellation risk.

4. **Booking volume should not be evaluated on its own.**
   A hotel or market segment may generate a large number of reservations while also showing a relatively high cancellation rate. Booking volume, cancellation rate, lead time and average daily rate provide a more useful picture when considered together.
