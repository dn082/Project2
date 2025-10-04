# Project2

## INTRODUCTION
In this project, I chose to analyze a data set that has information on coffee consumption data using the Global Coffee Health dataset. My goal is to predict a person’s Stress_Level (Low, Medium, or High) and to create a predictive model using a Random Forest Tree Classifier to categorize stress levels based on their lifestyle habits and coffee consumption. 

Questions 
- Can lifestyle factors such as coffee intake, sleep hours, physical activity, age, and BMI accurately predict a person's stress level?
- Which features are most influential in determining stress levels?

## THE DATASET
The data I chose to use is a file found from Kaggle called https://www.kaggle.com/datasets/uom190346a/global-coffee-health-dataset.
My target variable is Stress_Level, and my main predictors would be Coffee_Intake, Caffeine_mg, Sleep_Hours, Sleep_Quality, Age, and BMI.
There are 16 columns and 10000 rows.

## PREPROCESSING
Some steps I took for preprocessing my data were to:
- Dealing with Non-Existent Data - Doing this step allowed me to use data that was relevant and existed to answer my questions and focus on columns that will contribute to my predictions. For this case, I removed a column as there was no information in it.
- Used Label Encoding - This step allows to convert labels I had in text form, that were Low, Medium, High, into a numerical format like 0, 1, 2 so the Random Forest Classifier could be able to process them.
- Used One Hot Encoding - Doing this step allowed all the columns to turn text categories into numbers that the Random Forest model can use, which is usually binary.
- Data Split -  This allowed me to train the Random Forest model with a training set that was 80% and a testing set that was also 20%. This allows it to deal with unseen data, to get a measure of how well the model truly understood the relationships between lifestyle habits and stress models

## VISUALIZATION/DATA UNDERSTANDING
To explore the data, I plan to use Countplots, Bar Plot, Scatter Plots, and Heat Map
- For Countplot,	I took the Stress_Level, which is my target, and wanted to see the Low, Medium, and High stress compared to something else. For this, I chose occupation as an example.
- For Bar Plot,	this is the most important as it answers the question for important features. My barplot is called Top 15 Features, which provides a frequency distribution of features like Sleep_Hours or Caffeine.mg to understand the most common habits.
- For Scatter Plot,	this allows a way to show the different habits and how two factors simultaneously interact across the three stress categories. It also shows clustering for which is more common.
- For HeatMap	is just a graph version of the Confusion Matrix, as it shows the model evaluation and accuracy of the Random Forest model for each stress category after training.

## MODELING
The model I use is a Random Forest Model. I used this because it is a strong use for classification using data that can handle different things. This model essentially builds multiple decision trees and combines their outputs to improve accuracy and reduce overfitting. Each tree is trained on a random subset of the data and features, and the final prediction is made by majority vote.
This was good for this project specifically, as much data was numerical and category-based, and another was how it could give the most important part I was asking, which was my question, that was which lifestyle factors most influence stress level?. This by itself allowed Random Forest a way to measure how important each feature is in predicting the target variable. 

## EVALUATION
For this project, I tested 20% of the data, which was 2000 rows of information. The Random Forest Model performed well, as I used metrics shown in the classification report, which were for this project accuracy is 1.00, meaning 100%, and precision, recall, and F1-score were also 1.00 across Low, Medium, and High stress levels, and the Confusion Matrix is everything classified right as all stress levels were predicted correctly. Showing that the model was able to perfectly classify stress levels based on the features. I used these metrics because it's a strong predictors of whether the model is doing well, as accuracy tells the correctness of predictions. Precision shows what is actually correct. The recall	shows stress levels were correctly identified, and the confusion matrix shows how it was classified correctly.

## STORY
As I explored this dataset, the main question that I had, as it had a column specifically for Stress_Level, was how does coffee consumption, in general, affect a person's stress level, and how does its influence compare to other overall lifestyle habits?. From my analysis of the Global Coffee Health dataset it revealed through visualization that stress levels aren't fully dependent on the consumption of coffee, but it is a consideration. With all the features from the barplot, the highest one was rest/sleep, which was the most influential. The Random Forest Classifier provided a clear answer by ranking the features by their predictive power any form related to sleep was the highest, like Sleep_Hours and Sleep_Quality. There were many different ones after the one hot encoding, making the columns go from 16 to 38. The second most important factors were Caffeine_mg and Coffee_Intake. This indicates that the consumption habit has some level of stronger predictive signal for stress than the other health factors. The third most important factors were related to physical health, specifically BMI and Physical Activity Hours. The data on some level can show a skew because of the idea that, due to lack of sleep, there can be a larger coffee intake for getting daily energy. This can reframe the problem of stress levels, as what we consume can come from just a general imbalanced lifestyle that neglects sleep and activity. 

## IMPACT
I think the possible general impact can be a level of insight, as the predictive model and feature importance analysis offered important info on factors and can change the idea that the concept of having high stress levels due to consumption of coffee or anything in general can be unlikely and reframe it to where Sleep Hours could be in correlation of possibility of bad physical activity and caffeine consumption as habit.  The lack of perspective can skew it, though, as  unconsidered parts, such as not having enough time, can lead the fewer sleep hours, which can come from responsibilities like occupation, and energy levels can be affected due to age because of the decrease. There can be many other correlations that can just overall cause the lack of sleep, leading to high stress levels that can not be seen through just this data.

## REFERENCES
- This project was used using Jupyter Notebooks and was coded in Python with libraries such as Pandas, Matplotlib, Seaborn, and Scikit.
- The dataset used was [Global Coffee Health Dataset](https://www.kaggle.com/datasets/uom190346a/global-coffee-health-dataset) and the overall structure of this project should be
  *  `PROJECT2.ipynb`: My main code that has the data preprocessing, analysis, and visualization information. `synthetic_coffee_health_10000.csv`: The raw dataset file.

## TO VIEW VISUALIZATIONS 
- Click on the file `PROJECT2.ipynb` and Preview and scroll to see visualizations.

## TO RUN THIS PROJECT
- Download Zip Locally
- Download the raw dataset file from [Global Coffee Health Dataset](https://www.kaggle.com/datasets/uom190346a/global-coffee-health-dataset)
- Open Zip
- Move the raw dataset file you got from the  [Global Coffee Health Dataset](https://www.kaggle.com/datasets/uom190346a/global-coffee-health-dataset) to the Project2-main folder
- Open Visual Studio Code
- Download the extensions Python and Jupyter if you don't have them already installed
- Open the file using Visual Studio Code
- Run the Code
- Download required modules
- View the Visualizations





