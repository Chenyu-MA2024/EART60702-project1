# Project Reflection
------------------------------------
**Not finished yet...**  


# 1


# 2


# 3 Correlation Analysis  
This analysis employed correlation and linear regression to explore the relationships between various meteorological variables and temperature. Our scatter plot matrix and kernel density estimates indicate that most variables have a positively skewed distribution, and overall, the linear correlations are weak. Notably, temperature and humidity show a significant positive correlation. However, since meteorological principles often suggest a more complex relationship between temperature and relative humidity, it's crucial to verify the definition of QBOT (e.g., whether it represents specific or absolute humidity) and integrate domain knowledge into our interpretation.  
In the univariate linear regression, humidity explained a substantial portion of temperature variation (R² = 0.768), compared to shortwave radiation (R² = 0.367). Given that the scatter plots reveal a curved relationship, using Spearman correlation might capture the association more effectively than Pearson correlation. Moreover, the multivariate regression, which included additional variables, increased the explained variance to 93%, with low multicollinearity as indicated by VIF values near 1.   
To enhance the analysis, first, review and clarify the definition of QBOT to ensure it accurately reflects the intended humidity measure. Second, given the curved relationship observed in the univariate analysis, consider adopting Spearman correlation or non-linear modeling techniques, which may better capture the underlying dynamics. Integrating these adjustments with robust domain knowledge will lead to a more accurate and meaningful interpretation of the meteorological data.


# 4 Result & Future Work
From the results, we found that temperature is the most strongly correlated factor, particularly with shortwave radiation and the Lowest Model Level Water Vapor Mixing Ratio(QBOT). Additionally, our findings suggest that temperature is projected to increase by approximately 3 degrees Celsius between 2006 and 2080, while rainfall is also expected to increase, indicating a rising trend in extreme weather events over time. However, based on the professor's feedback on other groups' presentations, we realised that determining whether this constitutes an extreme weather trend requires a clearer definition of 'extreme weather'. Moving forward, we should conduct a literature review to establish a precise definition, ensuring that our analysis remains unbiased and that our conclusions are both rigorous and reliable.

For the future work section, we identified some areas for improvement. Incorporating additional features, such as air quality factors (PM2.5 concentration, CO₂ levels, ozone levels) and geographical factors (elevation, land cover type), could enhance the accuracy of our analysis. Feature selection techniques, including correlation analysis and multicollinearity checks, will be refined. Furthermore, advanced modelling approaches, such as regression models (Random Forest Regression) and deep learning models (Artificial Neural Networks and Time Series Forecasting) will be explored using historical data to improve predictive ability. The final model will then be used to predict key environmental factors, such as temperature and QBOT, to provide deeper insights into climate trends. 

During the presentation, we mistakenly considered humidity to have the same meaning as QBOT. This experience highlighted the importance of accurately understanding variable definitions to ensure the correctness of our conclusions. It also reinforced the necessity of careful data interpretation and validation of variable meanings in future analyses.
