# India CPI Analysis (Excel & Pivot Tables)

A case-study project analysing India's Consumer Price Index (CPI) from January 2013 to May 2023 using Microsoft Excel and Pivot Tables only (no SQL/Python).

## Dataset
- Monthly CPI index values for Rural, Urban and Rural+Urban sectors across 28 categories (Cereals, Meat & fish, Housing, Fuel & light, Health, Education, etc.) plus the General Index.
- Crude oil (Brent) daily prices from FRED: https://fred.stlouisfed.org/series/dcoilbrenteu

## Data Cleaning Steps
1. Filled missing values (e.g., April-May 2020 lockdown months) using a 3-period moving average; fixed errors/blanks manually using (upper + lower) / 2.
2. Removed individual Clothing and Footwear columns and kept the combined column.
3. Grouped categories into 5 buckets: Food, Clothing & Footwear, Housing, Fuel & Light, Miscellaneous.
4. Focused on the combined Rural+Urban series, since Rural and Urban showed very similar trends.
5. Added a Month_year column to sort pivot tables chronologically.
6. April 2019 data was unavailable and was skipped.

## Analysis Done
1. Category contribution: Food bucket has the largest share of the index, followed by Miscellaneous.
2. Year-wise comparison of all five buckets (2017-2023).
3. Individual food item inflation (June 2022 to May 2023): Spices rose the most (about +16%), Oils & fats fell the most (about -15%).
4. COVID-19 impact (2020): monthly trend of Food, Fuel & Light, Health and Transport.
5. Crude oil vs CPI: monthly average oil prices compared with category changes using correlation (2021-2022).

## Tools Used
Microsoft Excel: Pivot Tables, formulas (AVERAGE, CORREL), sorting, data cleaning.

## Limitations
- Moving-average smoothing was applied to the series, so values differ slightly from the official published index.
- Category index values were added together for the contribution analysis. This is a simple, unweighted approach, not the official weighted CPI method.
- 2023 has only 5 months of data, so year-wise totals are not directly comparable with full years.
- Correlation with crude oil uses a short window (2021-2022) and shows association, not causation.

## Files
- INDIA_CPI case study assignment.xlsx: raw data, cleaned data, pivots and analysis sheets.

## Author
Akhilesh | Learning data analytics
