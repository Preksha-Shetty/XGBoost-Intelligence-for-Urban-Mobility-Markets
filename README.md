# NYC-RideHailing-Market-Intelligence-XGBoost

Optimizing Driver Revenue & Reducing Marketplace Friction in a 50M+ Record Dataset

Project Overview
This project addresses the 79.6% take-home pay efficiency gap in the New York City High-Volume For-Hire Vehicle (Uber/Lyft) marketplace. Using a massive dataset of 221 million raw records (aggregated to 1.07 million rows), I developed a predictive intelligence system to help drivers maximize earnings and assist platforms in identifying service gaps.

Key Predictive Objectives
Objective A: Market Categorization (Classification)

Goal: To predict the "grade" of any neighborhood-hour block.

Output: Categorized zones into High Tip, High Fare, and Low Yield to guide drivers toward lucrative opportunities.

Objective B: Driver Pay Optimization (Regression)

Goal: To predict driver_pay and identify the "Sweet Spot" for revenue.

Insight: Statistically proved that Trip Distance is the #1 predictor of pay, outweighing location and time.

Objective C: Destination Profitability (The "Look-Ahead")

Goal: To predict the future revenue potential of a trip’s Drop-off Zone (DOLocationID).

Value: Helps drivers avoid "drifting empty" by evaluating a destination's value before accepting the ride.

Objective D: Supply Desert Analysis (Matching Friction)

Goal: To predict passenger wait_time across the city.

Impact: Pinpointed "Supply Deserts" occurring predictably between 2:00 AM – 5:00 AM, providing a roadmap for platform incentives.

The Tech Stack
Data Processing: Python (Pandas, NumPy)

Machine Learning: XGBoost (Regressor & Classifier), Scikit-Learn

Visualization: Seaborn, Matplotlib (Enhanced for high-density storytelling)

Data Scale: 221M raw records / 1.07M processed rows

Analytical Rigor & Results
Validation: Utilized an 80/20 train-test split with Mean Absolute Error (MAE) and Accuracy Scores to ensure model reliability.

Feature Engineering: Engineered custom features including wait_time, day_of_week, and rev_per_mile to uncover non-linear market patterns.

Performance: Achieved high overlap in "Actual vs. Predicted" density curves, proving the model accurately mirrors NYC's volatile market patterns.

Data Access: Due to the million row scale, the raw CSV is not hosted here. Data can be sourced from the NYC TLC Open Data Portal.
