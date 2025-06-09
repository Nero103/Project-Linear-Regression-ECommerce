# Project-Linear-Regression-ECommercet.

# Overview
This is a Linear Regression project on e-commerce data from Kaggle. The model is used to see which platform the company provides has the most association with the total amount spent by customers. By doing this analysis, the model can predict which feature (variable/column) will result in an increase in the total amount spent.

# Background
A company has recently built a website and app for customers to use when wanting an on-demand shopping experience. The company came across fluxuating sales from the website and app. So, they needed to know which platform, website or app, to focus on developing based on the revenue generated from each platform experience. A predictive model was determined to be best at identify the likelihood of revenue generation based on several key variables

# Project Goal
To build a linear regression model that predicts Yearly Amount Spent by customers based on usage patterns, and to determine whether the mobile app or the website has a stronger impact on revenue. Ultimately, this insight will inform decision-makers and drive business strategy on where to allocate resources for greater return on investment.

# Tools Used
- Python
- Libraries: pandas, numpy, seaborn, matplotlib, scikit-learn

# Data Cleaning
- The dataset was loaded using pandas to perform easier data manipulation and cleaning upon the variables. The was no missing values but some feature transformation were done.
- Basic descriptive statistics and data exploration were performed.
- No advanced cleaning was needed as the dataset was relatively mostly clean.

# Analysis
Exploratory Data Analysis (EDA) was performed using seaborn and matplotlib to explore Length ofMembership, Time on App, Time on Website, and Avg. Session Length:

- Pairplots revealed linear relationships between some variables.
- Correlation analysis showed that Length of Membership was most strongly correlated with the Yearly Amount Spent.
- Visualization & Interpretation
- Pairplots helped visualize relationships between variables.
- Heatmaps showed strong correlations between numerical variables.
- Regression plots indicated:
- Length of Membership and Yearly Amount Spent had the strongest linear relationship.
- Mobile App usage showed a slightly higher positive correlation with yearly spending than Website usage.

# Modeling
A Linear Regression model was trained using scikit-learn. Features included: Avg. Session Length, Time on App, Time on Website, and Length of Membership. The dataset was split into training and testing sets (70/30 split).

Model performance metrics:
- Mean Absolute Error (MAE)
- Mean Squared Error (MSE)
- Root Mean Squared Error (RMSE)

# Results & Findings
The regression model had a high R² score of 0.98, indicating a good fit. Length of Membership was the most significant predictor of yearly spending at a coeficient of 61.5. Meanwhile, Time on App (coeficient 38.70) was a more relevant predictor than Time on Website (coeficient 0.43).

Coefficients:
- Time on App had a positive coefficient, suggesting higher app usage leads to more spending.
- Time on Website had a negative or negligible coefficient.

# Recommendations for Business
Invest in improving the Mobile App experience to increase user engagement and revenue. Optimize app features such as personalization, promotions, and faster checkout. Likewise, consider deprioritizing the website or focusing on improvements that enhance app transitions.
Furthermore, analyze customer loyalty programs, as Length of Membership is a strong predictor of spending.
