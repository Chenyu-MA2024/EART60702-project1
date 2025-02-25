# Project Reflection
------------------------------------



# 1


# 2 Pre-processing
The data preprocessing phase prioritised ensuring data integrity by confirming the absence of missing or duplicate values, correcting inaccuracies, and interpolating negative precipitation and snowfall values. Temperature was converted from Kelvin to Celsius, and longitude was adjusted from a 360-degree format to -180 to 180 degrees, identifying Manchester as the dataset's location. Time attributes were expanded to facilitate seasonal analysis. Additionally, variable names were altered for ease of interpretation for non-experts as this type of data is common to present to governments and other organizations for climate mitigation strategies. 

A comparison with the CHESS Regional Climate Model (RCM) from the UK Centre for Ecology & Hydrology (CEH) revealed similar temperature trends. Both project a 3°C increase. The CHESS dataset uses moderate climate scenarios with no climate change mitigation, which could mean our data presents a similar scenario. This consistency suggests analogous preprocessing methodologies, though further validation is necessary.

An important insight emerged regarding the misinterpretation of the QBOT variable, initially assumed to represent humidity but actually denoting water vapour. This highlights the importance of rigorously verifying dataset definitions and incorporating domain-specific expertise to enhance analytical accuracy. The preprocessing efforts established a robust foundation for subsequent analysis, ensuring data consistency and reliability. The alignment with CHESS findings reinforces the validity of the approach while identifying areas for further investigation into climate projections.


# 3 Correlation Analysis  
This analysis employed correlation and linear regression to explore the relationships between various meteorological variables and temperature. Our scatter plot matrix and kernel density estimates indicate that most variables have a positively skewed distribution, and overall, the linear correlations are weak. Notably, temperature and humidity show a significant positive correlation. However, since meteorological principles often suggest a more complex relationship between temperature and relative humidity, it's crucial to verify the definition of QBOT (e.g., whether it represents specific or absolute humidity) and integrate domain knowledge into our interpretation.  

In the univariate linear regression, humidity explained a substantial portion of temperature variation (R² = 0.768), compared to shortwave radiation (R² = 0.367). Given that the scatter plots reveal a curved relationship, using Spearman correlation might capture the association more effectively than Pearson correlation. Moreover, the multivariate regression, which included additional variables, increased the explained variance to 93%, with low multicollinearity as indicated by VIF values near 1.   

To enhance the analysis, first, review and clarify the definition of QBOT to ensure it accurately reflects the intended humidity measure. Second, given the curved relationship observed in the univariate analysis, consider adopting Spearman correlation or non-linear modeling techniques, which may better capture the underlying dynamics. Integrating these adjustments with robust domain knowledge will lead to a more accurate and meaningful interpretation of the meteorological data.


# 4 Result & Future Work
From the results, we found that temperature is the most strongly correlated factor, particularly with shortwave radiation and the Lowest Model Level Water Vapor Mixing Ratio(QBOT). Additionally, our findings suggest that temperature is projected to increase by approximately 3 degrees Celsius between 2006 and 2080, while rainfall is also expected to increase, indicating a rising trend in extreme weather events over time. However, based on the professor's feedback on other groups' presentations, we realised that determining whether this constitutes an extreme weather trend requires a clearer definition of 'extreme weather'. Moving forward, we should conduct a literature review to establish a precise definition, ensuring that our analysis remains unbiased and that our conclusions are both rigorous and reliable.

For the future work section, we identified some areas for improvement. Incorporating additional features, such as air quality factors (PM2.5 concentration, CO₂ levels, ozone levels) and geographical factors (elevation, land cover type), could enhance the accuracy of our analysis. Feature selection techniques, including correlation analysis and multicollinearity checks, will be refined. Furthermore, advanced modelling approaches, such as regression models (Random Forest Regression) and deep learning models (Artificial Neural Networks and Time Series Forecasting) will be explored using historical data to improve predictive ability. The final model will then be used to predict key environmental factors, such as temperature and QBOT, to provide deeper insights into climate trends. 

During the presentation, we mistakenly considered humidity to have the same meaning as QBOT. This experience highlighted the importance of accurately understanding variable definitions to ensure the correctness of our conclusions. It also reinforced the necessity of careful data interpretation and validation of variable meanings in future analyses.
