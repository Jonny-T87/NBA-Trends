# NBA-Final Home Team Wins Predictive Model 

**Jonny Tesfahun**

# Trends in NBA Home Team Wins:
## The analysis of NBA Finals statistics which are likely to lead a Home Team to Win

Brief Description of Data:

The data is a collection of NBA Finals games data from the 2004 season to dec 2020 season. The file contains all games home and away data. Some of these include home points, away points, FG percent home & away, FT percent home & away.

### Objective Goal:

The goal of the data is to predict the likelihood a home team will win during a game. Thus, how accurately can the model predict Home_Team_Wins? which is the target of the dataset. 

### Business problem:

What factors lead to Home Team Win?\
What is the Avg. Assist that leads to Home Team Win?\
What is the Avg. Rebound that leads to Home Team Win?\
Do high FG% lead to Home Team Win?
Do high FT FG% lead to Home Team Win?
Do high 3pt FG% lead to Home Team Win?
Does a game played in a certain month mean more likely to lead to Home Team Win?


### Data:
Source of file is included below: \
https://www.kaggle.com/datasets/nathanlauga/nba-games?select=ranking.csv  \
Source of data: \
Using games.csv file.


## Methods
- Cleaned the data for any Errors and or Inconsistencies
- Used Histogram, Boxplot, Heatmap, and Pair Plot for Visual Exploratory Data Analysis
- Incorporated Informative Multivariate Presentation Visuals for Closer Analysis of Data 
- Adopted Logistic Regression and Decision Tree Classifier Models to data
- Included Principal Component Analisis (PCA) with and without for both Models
- 1st Evaluated performance of the models based on Accuracy
- 2nd Evaluated performance of the models based Precision, Recall, and F1 Score, 
- 3rd Evaluated performance on some models is Grid Search CV. 

## Results 

All of the 4 different models (Logistic Regression & Decision Tree Classifier) with and without Principal Component Analisis (PCA) tested very well on the data set. Especially since it is predicting an actual future outcome from past game statistics, which is Home Team Wins. 

The best model out of my analysis was the tuned Logistic Regression with no PCA. Slight tuning of each model hyperparameters was able to increase data prediction accuracy and lower overfitting of the data. The accuracy on the testing data had a little increase over the previous model and was 60.02%. The F1 score was slightly lower than the previous model with 73.57%, also the Recall was slightly lower at 93.55%. However, the small increase in Accuracy made-up for this. 

#### Visual 1 - Home Points Scored per Season Vs. Wins & Losses
![My Image](https://github.com/Jonny-T87/NBA-Trends/blob/main/nba_trends.png)

> "
> 
#### Visual 2 - Actual Home Points Scored per Season vs Avg. Home Points Scored per Season
![My Image](https://github.com/Jonny-T87/NBA-Trends/blob/main/nba_trends_2_points.png)

> "


## Model

The tuned Logistic Regression with no PCA model was the best. Slight tuning of each model hyperparameters was able to increase data prediction accuracy and lower overfitting of the data. The parameters used were C=0.1, max_iter = 1000, solver = 'liblinear', penalty = 'l1'. With these parameters, the accuracy on the testing data had a good increase over the previous model and was 60.02%. The F1 score was slightly lower than the previous model with 73.57%, also the Recall was slightly lower at 93.55%. However, the small increase in Accuracy made-up for this. The Precision score was 60.62% which was one of the highest out of all the models.

In addition, Grid Search CV was also used on the Logistic Regression model without PCA. However, Grid Search did not out perform the above model. 

This Model and the Parameters together would solve many complex NBA Statistic problems. For Instance, increasing the playing style of team to induce more Home Assist and 3pt FG% which in turn leads to more Home Team Wins. These Home Team Wins can help the team create a bigger fan base and sale more home tickets at higher prices. 

## Recommendations:

From the information above, Logistic Regression slightly outperformed Decision Tree Classifier using Grid Search. Many changes can be made to parameters or inputs to increase Accuracy but the cost may be CPU performance. A recommendation for future models with this type of prediction, would be to utilize Randomized Search CV. This would help in finding the best hyperparameters and inputs for the most accurate possible prediction of Home Team Win.

I would also recommend PCA not be used in the models. This would also avoid losing key features in the data that are correlated to the target. In addition, more data can be added if overfitting is still a concern. 


### For further information

For any additional questions, please contact **jonnymtesfahun@gmail.com**
