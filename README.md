# econ3916-lab19-random-forests

# Tree-Based Models: Random Forests

## Objective

I explored how tree-based models predict housing prices and how feature importance helps explain model predictions.

## Methodology

- I used the California Housing dataset and split it into training and test sets.
- I fitted a single decision tree, OLS, Ridge, and a random forest, and compared their performance using RMSE and R².
- I compared impurity-based importance (MDI) and permutation importance to understand how each method measures feature importance.
- I used cross-validation to tune the random forest and evaluated the selected model on the test set.
- I wrote my own prompt asking AI to create a feature-importance chart function, revised it over two rounds, and checked its results against my own calculations.

## Key Findings

- The single decision tree had a test R² of 0.6228, while OLS and Ridge both had a test R² of 0.5758. The random forest performed better, with a test R² of 0.8046.
- Latitude had an MDI importance of 0.0890 but a permutation importance of 0.4427. I learned that different importance measures can give different views of the same feature.
- After tuning the random forest through cross-validation, the test R² increased slightly to 0.8094.
- Both rounds of AI-generated code passed all numerical checks with a 0% difference. In the second round, I added four-decimal-place labels to the charts without changing the returned values.
- I learned that AI can help me write reusable chart code, but I still need to check its calculations and visual output before trusting it.
