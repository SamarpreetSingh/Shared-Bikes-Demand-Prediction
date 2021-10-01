# Shared-Bikes-Demand-Prediction

kaggle - https://www.kaggle.com/c/shared-bikes-demand-prediction

This is a kaggle competition project of Data science and Artificial intelligence.

A US bike-sharing provider `XBikes` has a daily dataset on the rental bikes based on various environmental and seasonal settings. It wishes to use this data to understand the factors affecting the demand for these shared bikes in the American market and come up with a mindful business plan to be able to accelerate its revenue as soon as the ongoing lockdown due to corona pandemic comes to an end.

Essentially, the company wants to know —
- Which variables are significant in predicting the demand for shared bikes.
- How well those variables describe the bike demands
- Predict the count of Bikes used.

Solution: 

I have removed features like "instant" and "dteday" which did not had much relevance while predicting the count of bikes. Then I have calculated the correlation values and chi-square values. "holiday" and "workingday" had low correlation values (less than 0.2) and high chi-square values, so they are also dropped from the features. 
Then I have used sklearn library to fit linear regression model to our data which performs really well.
