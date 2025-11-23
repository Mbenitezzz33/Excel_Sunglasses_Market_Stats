### Project Overview
This project analyzes a real dataset of 259 Amazon best-selling sunglasses from 2024. All work is completed in Excel using active formulas to ensure transparency and reproducibility.

The analysis follows the requirements from CIDM/FIN 4308 – Data Analytics for Business and includes:

- Data cleaning and preparation
- Summary statistics
- Histogram visualizations
- Correlation analysis
- Multiple regression
- Two-sample t-test
- Managerial conclusions and insights

Final workbook: Matthias_Benitez_Sunglasses_Market_Stats.xlsx

### Part A — Summary Statistics & Visuals
Located in the Summary tab.

#### Variables analyzed
- price
- rating
- reviews
- ln_reviews

#### Summary table includes
- Count
- Mean
- Median
- Standard deviation (STDEV.S)
- Min & Max

#### Histograms
- Price Histogram — Right-skewed, with most items priced under ~$35.
- Rating Histogram - The histogram captures the tight clustering of ratings around 4.2–4.6.

#### Key insights
- Ratings have extremely low variance; most sunglasses are rated very highly.
- Review counts are heavily skewed, supporting the use of the log transformation (ln_reviews).
- Price varies far more than rating, indicating more diversity in cost tiers.

### Part B — Correlation & Regression
Located in the Regression tab.

#### Model
ln(reviews) = a + b_price * price + b_rating * rating

#### Output includes
- Coefficients
- p-values
- Confidence intervals
- Standard errors
- Adjusted R²

#### Interpretation
- b_price: Small, negative coefficient. Holding rating constant, higher-priced sunglasses receive slightly fewer reviews. Effect size is extremely small due to the log scale.
- b_rating: Positive coefficient. Higher ratings correspond to more reviews, but the effect is still weak.
- Adjusted R²: Low. Price and rating alone do not strongly predict review volume; external factors like branding and visibility likely dominate.

### Part C — Hypothesis Test (High-Price vs Low-Price Ratings)
Located in the Hypothesis tab.

#### Grouping rule
high_price = 1 if price ≥ median(price)
high_price = 0 otherwise

#### Test used
Two-sample, two-tailed t-test assuming equal variances.

#### Results
- t-statistic: -0.352887852 
- p-value (Tw0 Tailed): 0.724930401
- Decision: Fail to reject the null hypothesis at α = 0.05
- Conclusion: Ratings for high-priced and low-priced sunglasses are statistically the same. Price does not meaningfully influence customer ratings.

#### Managerial interpretation
Customers do not rate expensive sunglasses higher than cheaper ones. Product attributes such as style, branding, and usefulness likely matter more than price.

### Repository Contents
- Matthias_Benitez_Sunglasses_Market_Stats.xlsx — Full Excel analysis with active formulas
- README.md — Project summary and walkthrough

### Skills Demonstrated
- Data cleaning & filtering
- Excel summary statistics
- Histogram construction & bin adjustment
- Correlation analysis
- Multiple regression (ToolPak)
- Two-sample t-testing
- Analytical storytelling & interpretation
<img width="1491" height="907" alt="Capture HW1_Github" src="https://github.com/user-attachments/assets/033f471a-0551-4083-add6-7d248186685d" />
