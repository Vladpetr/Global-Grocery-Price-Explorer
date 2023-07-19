# Global-Grocery-Price-Explorer
Explores and models the cost of groceries in different regions, investigating variations based on country, store brand, and potential correlations with rental prices.

## Project Overview
In this project, I answered the following key questions:

1. What is the average price of each product, and how do we anchor it considering different currencies and price distributions?
2. How does the geographical location of grocery stores affect product prices, and how does the store brand classification (budget, mid-range, or luxury) influence these variations?
3. Is there a correlation between price variation by geographical location and rental prices in the corresponding neighborhoods?
4. Can we enhance our analysis by incorporating a spatially correlated distribution over location multipliers to reveal underlying patterns in price fluctuations?
## Data
To conduct the analysis, I collected price data for ten essential grocery items from various supermarkets across different countries. Each product has three recorded prices, accounting for brand variations. Additionally, I recorded the quantity of each product to standardize the prices.

To establish correlations, we sourced rental price data for the neighborhoods where these supermarkets are located.

I also explored the incorporation of a spatially correlated distribution over location multipliers. This modification allowed me to investigate hidden patterns in price variations, considering the spatial proximity of grocery stores.

## Model Implementation
I used PyStan to build the model. The model structure is based on a combination of a base price for each product and multipliers associated with store brands and geographical locations. This allows us to predict the final price of a product in a particular store effectively.
