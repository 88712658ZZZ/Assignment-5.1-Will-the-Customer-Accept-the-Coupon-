# Driving Coupon Acceptance Analysis

## Project Overview
This project investigates the factors that influence whether a driver will accept a mobile coupon for a local business while driving. Using data from the UCI Machine Learning Repository, we explore various scenarios—including destination, weather, time, and passenger demographics—to identify the characteristics of customers who are likely to engage with these offers.

## Summary of Findings

### 1. General Acceptance
- The overall coupon acceptance rate across all categories (Restaurants, Coffee Houses, Bars, etc.) is approximately **57%**.
- **Carry Out & Take Away** and **Inexpensive Restaurants** show the highest baseline acceptance rates.

### 2. Bar Coupon Insights
- **Habit is Key:** Drivers who visit bars more than 3 times a month are significantly more likely to accept a bar coupon (approx. 76%) compared to those who visit rarely (approx. 37%).
- **Age Demographics:** Drivers under the age of 30 accept bar coupons at a higher rate than older age groups.
- **Social Context:** Drivers with passengers who are not children (e.g., friends or partners) show a higher propensity for detouring to a bar.

### 3. Independent Investigation: Coffee House Coupons
- **Time of Day:** Coffee house coupons see a peak in acceptance during the 10 AM and 2 PM windows, aligning with mid-morning and mid-afternoon breaks.
- **Environment:** Sunny weather significantly boosts the likelihood of a driver stopping for coffee compared to rainy or snowy conditions.
- **Occupation:** Students and those in sales-related roles were found to be more responsive to coffee house offers than those in highly structured corporate environments.

## Actionable Recommendations
- **Dynamic Timing:** Deliver Coffee House coupons specifically during the 10 AM window on sunny days to maximize conversion.
- **Behavioral Targeting:** Prioritize Bar coupons for users who have a historical frequency of visiting similar venues, especially during evening trips where no urgent destination is set.
- **Contextual Filtering:** Avoid sending Bar coupons to drivers with children as passengers, as the data shows a sharp decline in acceptance for this segment.

## Repository Structure
- `prompt.ipynb`: The main Jupyter Notebook containing data cleaning, visualizations, and statistical analysis.
- `data/coupons.csv`: The source dataset containing survey responses.
- `README.md`: Non-technical report and project summary.

## How to Run the Analysis
1. Clone the repository.
2. Ensure you have `pandas`, `seaborn`, and `matplotlib` installed.
3. Run the cells in `prompt.ipynb` to view the data processing and plots.
