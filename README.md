# Kraken Koffee Sales Infographic

This Power BI project presents a comprehensive sales analysis and forecasting dashboard for Kraken Koffee — a fictional Florida-based coffee chain. The infographic-style report visualizes half-year (Jan–Jun 2023) performance across store locations, product categories, time of day, and transaction patterns. It also includes a full-year sales forecast powered by advanced DAX measures.

---

## Project Objectives

- Summarize sales activity across three store locations
- Identify top-selling products and peak revenue hours
- Analyze customer buying behavior based on time of day
- Forecast year-end sales using current performance trends
- Present findings in a visually engaging, single-page infographic layout

---

## Dashboard Highlights

### Infographic Overview
- Total Sales, Transactions, Average Order Size
- Best-selling and top-earning products
- Heatmap and trend charts for daily/monthly performance
- FY 2023 sales forecast per store and overall

### Sales by Time of Day
- 56% of revenue is generated during morning hours
- Peak average order size at 8–10 AM
- Visual breakdown by hour and weekday

### Product & Category Insights
- Coffee and Tea lead sales by category
- **Davy Jones' Organic Hot Chocolate (Large)** is the top revenue earner
- **Crow’s Nest Croissant** is the most frequently purchased item
- Dynamic labeling and color highlights used to emphasize top performers

### Store-Level Performance
- Tampa store recorded the highest total sales (~$240K)
- Store-wise forecasting shown using clean line visuals with markers
- Comparative view of total and average order size per store

---

## DAX Measures Explained

This project relies heavily on DAX to drive dynamic logic, product ranking, visual formatting, and forecasting. Below is how each group of DAX measures adds value to the report:

### Core KPIs

- **`Total Sales`**: Aggregates revenue from all transactions; central to most charts and cards.
- **`Total Transactions`**: Measures customer traffic; supports AOS (Average Order Size).
- **`Total Products`** & **`Total Stores`**: Used for counts in infographic headers and filters.
- **`Average Order Size`**: Indicates customer spend per transaction; used in hourly visuals and as a summary metric.
- **`Top Earner`**: Identifies the highest revenue-generating product dynamically.
- **`Most Popular Seller`**: Shows the most frequently purchased product by transaction count.

### Ranking Measures

- **`Product Sales Rank`**: Ranks products by revenue for sorting and label logic.
- **`Product Transaction Rank`**: Ranks products by number of transactions.
- **`Product Category Rank`**: Used for conditional formatting and top 10 highlighting.

### Nested Logic & Visual Enhancements

- **`% of Sales`**: Calculates share of total sales per category/product — used in labels and tooltips.
- **`Max Avg Order Size (Hour)`**: Determines which hour had the highest average order size.
- **`Max AOS Marker`**: Used to place a marker only at the peak hour in time-based visuals.
- **`Bar Chart Label (Product Category)`**: Combines dollar and percent formats for intuitive bar chart labeling.
- **`Top 10 Product Type Highlight`**: Applies dynamic color based on ranking — gold for top 10, blue otherwise.
- **`MAX AOS Marker Label`**: Creates a labeled data card for the peak AOS hour.

### Forecasting Logic

- **`Average Daily Sales`**: Calculates base daily average sales.
- **`Average Daily Sales 2`**: Respects visual filters to produce consistent outputs.
- **`Average Daily Sales Switch`**: Smart logic to fallback on average where data is missing.
- **`Forecast`**: Main measure used to estimate FY 2023 sales based on trends.
- **`Forecast Label`**: Displays final projected sales cleanly on KPI cards.
- **`Forecast Marker`**: Used to highlight December data point in forecast line visuals.

---

## Dashboard Previews

### 1. Infographic Page

![Kraken_Koffee_Infographics](https://github.com/user-attachments/assets/6869acfd-5097-46c0-98ec-a72af03425f1)

### 2. Forecast View

![Forecast Visuals](https://github.com/user-attachments/assets/848f0232-39f3-4374-a35d-57622e8e3990)


### 3. Sales by Hour

![TimeVisuals](https://github.com/user-attachments/assets/0f4156cd-38f2-400e-9aa6-f2edba0a125a)

---

## Summary

This Power BI report empowers business users with dynamic sales insights, time-based performance views, and a full-year forecast — all presented through a clean, infographic-style layout. DAX plays a central role in making the report highly interactive and intelligent, from label formatting to visual rankings and future sales projection.
