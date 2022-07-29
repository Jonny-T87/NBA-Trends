# NBA-Trends

**Jonny Tesfahun**

# Trend in NBA Home Team Points Scored:
## The analysis of Home Points Scored Vs. Other Features Which are Likely to Lead Team to Win

Brief Description of Data:

The data is a collection of NBA games data from the 2004 season to dec 2020 season. The file contains all games home and away data. Some of these include home points, away points, FG percent home & away, FT percent home & away.

### Objective Goal:

The goal of the data is to predict the likelihood a home team will win during a game. Thus, how accurately can the model predict Home_Team_Wins? which is the target of the dataset. 

### Business problem:

What factors lead to Home Team Win?\
Having Home Team Points increased over the seasons?\
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
- Included Principal  Component Analisis (PCA) with and without for both Models
- 1st Evaluated performance of the models based on Accuracy, R2 score, Mean Squared Error (MSE), and Root Mean Squared Error (RMSE)
- 2nd Evaluated performance of the best model with the Precision, Recall, and F1 scores 

## Results 

All of the 4 different models (Logistic Regression & Decision Tree Classifier) with and without Principal Component Analisis (PCA) tested great on the data set.

The 2 models with PCA and no tuning did overall the worst with accuracy on the testing data between 82-91% and the coefficient of determination (r2) scores being low as well ranging from 25-61%. Meaning that it could only explain at most 61% of the variation in the target data of the model.

The next lowest models were also PCA but with some tuning of the Logistic Regression & Decision Tree Classifier hyperparameters. These two models had a slight increase in accuracy on the testing data being between 83-91%. They also had a slight increase in the r2 scores, being between 26-61%. 

The next best models were Logistic Regression & Decision Tree Classifier without tuning. Their accuracy on the testing data was between 99.37-99.56%. A dramatic increase. Their r2 scores were also high, being between 97.44-98.20%. The only issue with these models is a concern of overfitting that data. 

The best out of my analysis were the tuned Logistic Regression & Decision Tree Classifier models. Slight tuning of each model hyperparameters was able to increase data prediction accuracy and lower overfitting of the data. Their accuracy on the testing data had a little increase and was between 99.55-99.61%. The r2 scores also slightly increase being between 98.14-98.40%.  

#### Visual 1 - Home Points Scored per Season Vs. Wins & Losses
![My Image](https://github.com/Jonny-T87/NBA-Trends/blob/main/nba_trends.png)

> "
> 
#### Visual 2 - Actual Home Points Scored per Season vs Avg. Home Points Scored per Season
![My Image](https://github.com/Jonny-T87/NBA-Trends/blob/main/nba_trends_2_points.png)

> "


## Model

Overall, from my analysis and the models, the PCA did not increase accurate prediction of the models or accurately explain the variances. Thus, in my opinion the best model to implement is the tuned Decision Tree Classifier. This model also has the lowest r2 score, Mean Squared Error (MSE), Mean Absolute Error (MAE), and Root Mean Squared Error (RMSE). All of which are below 0.06. 

For the tuned Decision Tree Classifier, the Precision, Recall, and F1 scores were also high ranking. I used these 2nd results of testing the data to justify my choice. The Precision score shows 99.55% of the time the model intuitively shows the ability of the classifier not to label a negative sample as positive. The Recall score of 99.78% shows that the model is able to find almost all of the positive samples. In addition, with 99.66% F1 scores, the model compares the performance of two classifiers really well.

This Model and the Metrics together would solve many complex NBA Statistic problems. For Instance, increasing the playing style of team to induce more Home Assist and 3pt FG% which in turn leads to more Home Team Wins. These Home Team Wins can help the team create a bigger fan base and sale more home tickets at higher prices. 

## Recommendations:

This model should be used because it accurately predicts 99% of the Home Team Wins target on the Test data, which is close to perfect as it gets.

I would recommend PCA not be used in the models. This would also avoid losing key features in the data that are correlated to the target. In addition, more data can be added if overfitting is still a concern. 


### For further information

For any additional questions, please contact **jonnymtesfahun@gmail.com**
