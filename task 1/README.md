# Hotel Booking Data Analysis

This project analyzes 119,390 hotel reservations from City and Resort hotels, covering booking activity between 2015 and 2017.

The work started as a data cleaning and first-exploration task, but I extended it to examine cancellation behavior, booking channels, lead time and differences between hotel types.

## What I worked on

Using Python, pandas and Matplotlib, I:

* inspected the dataset structure, data types and missing values
* converted reservation dates to datetime format
* handled missing values based on the meaning of each column
* reviewed duplicate records instead of automatically removing them
* created `total_nights`, `total_guests` and lead-time groups
* used descriptive statistics and grouped analysis to explore booking behavior
* compared cancellation patterns across hotel types, market segments and lead times
* created visualizations for booking trends, reservation outcomes and cancellation behavior

One important cleaning decision was to **keep identical rows**. The dataset does not contain a unique booking ID, so automatically removing all duplicated rows could also remove valid reservations with identical characteristics.

* booking volume
* cancellation rate
* lead time
* average daily rate

Combining these indicators gives a more realistic view of booking quality and expected demand.

## Key Visualizations

The notebook includes:

* distribution of reservation outcomes
* booking volume by year
* booking volume by market segment
* cancellation rate by market segment
* cancellation rate by lead-time group
* comparison of lead time between canceled and non-canceled bookings
* histogram of average daily rate

## Tools

* Python
* pandas
* Matplotlib
* Jupyter Notebook

## Dataset

**Hotel Booking Demand**

The dataset contains anonymized booking information for one City Hotel and one Resort Hotel and includes customer, reservation, pricing and cancellation-related variables.
