# Boom-Bike-Sharing-LR-model
BoomBikes aspires to understand the demand for shared bikes among the people after this ongoing quarantine situation ends across the nation due to Covid-19.


A bike-sharing system is a service in which bikes are made available for shared use to individuals on a short term basis for a price or free. Many bike share systems allow people to borrow a bike from a "dock" which is usually computer-controlled wherein the user enters the payment information, and the system unlocks it. This bike can then be returned to another dock belonging to the same system.


A US bike-sharing provider BoomBikes has recently suffered considerable dips in their revenues due to the ongoing Corona pandemic. The company is finding it very difficult to sustain in the current market scenario. So, it has decided to come up with a mindful business plan to be able to accelerate its revenue as soon as the ongoing lockdown comes to an end, and the economy restores to a healthy state. 


In such an attempt, BoomBikes aspires to understand the demand for shared bikes among the people after this ongoing quarantine situation ends across the nation due to Covid-19. They have planned this to prepare themselves to cater to the people's needs once the situation gets better all around and stand out from other service providers and make huge profits.


They have contracted a consulting company to understand the factors on which the demand for these shared bikes depends. Specifically, they want to understand the factors affecting the demand for these shared bikes in the American market. The company wants to know:

Which variables are significant in predicting the demand for shared bikes.
How well those variables describe the bike demands
Based on various meteorological surveys and people's styles, the service provider firm has gathered a large dataset on daily bike demands across the American market based on some factors. 


### Q1. From your analysis of the categorical variables from the dataset, what could you infer about their effect on the dependent variable?


Ans: Here are some of the inferences I made from my analysis of categorical variables from the
dataset on the dependent variable (Count)
1. Fall has the highest median, which is expected as weather conditions are most optimal to ride
bike followed by summer.
2. Median bike rents are increasing year on as year 2019 has a higher median then 2018, it might be
due the fact that bike rentals are getting popular and people are becoming more aware about
environment.
3. Overall spread in the month plot is reflection of season plot as fall months have higher median.
4. People rent more on non-holidays compared to holidays, so reason might be they prefer to
spend time with family and use personal vehicle instead of bike rentals.
5. Overall median across all days is same but spread for Saturday and Wednesday is bigger may be
evident that those who have plans for Saturday might not rent bikes as it a non-working day.
6. Working and non-working days have almost the same median although spread is bigger for nonworking days as people might have plans and do not want to rent bikes because of that
7. Clear weather is most optimal for bike renting, as temperate is optimal, humidity is less, and
temperature is less.


### Q2. Why is it important to use drop_first=True during dummy variable creation?


Ans: Dummy variables will be correlated if you don't remove the first column (redundant). This
may have a negative impact on some models, and the effect is amplified when the cardinality is
low. Iterative models, for example, may have difficulty convergent, and lists of variable importance
may be distorted. Another argument is that having all dummy variables results in multi collinearity
between them. We lose one column to keep everything under control.
### Q3. Looking at the pair-plot among the numerical variables, which one has the highest correlation with the target variable?


Ans: “temp” and “atemp” has the highest correlation (0.63) with the target variable

### Q4. How did you validate the assumptions of Linear Regression after building the model on the training set?

Ans: The distribution of residuals should be normal and centred around 0. (The mean is 0). We test
this residuals assumption by producing a distplot of residuals to see if they follow a normal
distribution or not.
The residuals are scattered around mean = 0 as seen in the diagram below.
### Q5. Based on the final model, which are the top 3 features contributing significantly towards explaining the demand of the shared bikes?

Ans: The Following are the top 3 features contributing significantly towards explaining the
demands of the shared bikes:
1. temp (0.3821)
2. weathersit_drizzle (-0.3200)
3. year (0.2407)
