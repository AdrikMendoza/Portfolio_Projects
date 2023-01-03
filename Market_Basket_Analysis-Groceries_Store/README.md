# Market Basket Analysis - Groceries Store

Market Basket Analysis is a powerful tool for translating vast amounts of customer transaction and viewing data into simple rules for product promotion and recommendation.

In this project we are going to find the most common and general rules for a Groceries Store. In order to make recommendations to put together certain products and offers.

# Conclusions

**After performing the Market Basket Analysis (MBA), we can conclude the next points:**

1. Using a min_support of 0.1 and prunning the data using Zhang's metric greater or equal to 0.15 and Confidence greater or equal to 0.35.
2. The most common item rules in the analysis are: Other Vegetables, Whole Milk, Rolls/Buns, Yogurt, Bottled Water.
3. After prunning rules we/ve found the top 10 rules.
4. `rolls/buns`, `whole milk`, `other begetables` are more likely to be the consequent item.

# Recommendations

1. These rules can be a good indicator to create "On Sale" promotions in order to increase sales.
2. Apply a recommendation engine to the end user.
