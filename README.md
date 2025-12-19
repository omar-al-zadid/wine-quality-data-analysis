# wine-quality-data-analysis
This short project identifies the statistically significant predictors of wine quality, and performs residual analysis and leverage analysis in order to validate linear regression assumptions.

# Methods
- Performed OLS-based multiple linear regression with t-test on a wine quality data with 1599 observations with wine quality as the response variable and 11 others as predictors.
- Plotted fitted vs residuals and leverage plots.
- Tried a few interaction effects between some predictors.

# Tools
Python, Jupyter Notebook, pandas, numpy, matplotlib, statsmodel

# Key results
- All the predictors except volatile_acidity show a statistically significant relationship to wine quality.
- Fitted vs residuals plot displays a mild funnel shape from left to right suggesting a possible unequal variance or heteroskedasticity. However, the pattern is too mild to be of concern.
- Several points are far from zero in y-axis indicating a possibility of them being outliers, especially for larger fitted values.
- Leverage plot shows several points with unusually high leverage. The outlier with the maximum leverage is the 151st observation.
- The interaction between citric_acid and residual_sugar is statistically significant when predicting alcohol level.
- The interaction between chlorides and total_sulfur_dioxide is statistically significant when predicting alcohol level. 
