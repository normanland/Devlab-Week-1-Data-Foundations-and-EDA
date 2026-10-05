# DevLab Week 1 — Data Foundations & Exploratory Analysis

Week 1 focused on moving from raw datasets to structured, business-oriented analysis using Python.

Rather than treating the exercises as isolated notebook tasks, I used three different datasets to practice the full early-stage analytics workflow: inspecting data quality, making cleaning decisions, exploring patterns, building visualizations, and translating results into practical observations.

## Analyses

### 01 · Hotel Booking Cleaning & Exploration

A 119,390-row hotel booking dataset was used to explore the foundations of data preparation and first-stage analysis.

The work covers missing-value treatment, duplicate assessment, feature creation, descriptive statistics, and cancellation behavior across hotel types, booking channels, and lead-time groups.

**Key question:** What factors help explain booking stability and cancellation behavior?

`Python` `pandas` `Matplotlib` `Data Cleaning` `EDA`

---

### 02 · Supermarket Sales EDA

A transaction-level supermarket dataset was analyzed across branches, product lines, customer types, and time of day.

The analysis compares revenue and transaction volume, identifies peak shopping periods, and examines how performance differs across business segments.

**Key question:** Where and when is supermarket sales activity concentrated?

`Python` `pandas` `Matplotlib` `Seaborn` `EDA`

---

### 03 · Istanbul Retail Multidimensional Analysis

Nearly 100,000 retail transactions were explored across product categories, shopping malls, payment methods, gender, and time.

The analysis extends beyond basic EDA through pivot-based comparisons, location and category performance, payment behavior, and month-over-month checks.

**Key question:** Which categories, locations, and customer patterns drive retail revenue?

`Python` `pandas` `Retail Analytics` `Pivot Analysis` `Business Insights`

---

## Week 1 Focus

The three analyses build on the same core workflow:

**inspect → clean → transform → explore → visualize → interpret**

The main objective was not only to produce charts, but to develop a repeatable way of approaching unfamiliar datasets and connecting analytical results to business questions.

## Repository Structure

```text
01-hotel-booking-cleaning-and-exploration/
02-supermarket-sales-eda/
03-istanbul-retail-multidimensional-analysis/
