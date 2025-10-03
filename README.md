# Project2

## INTRODUCTION
In this project, I chose to analyze a data set that has information on coffee consumption data using the Global Coffee Health dataset. My goal is to predict a person’s Stress_Level (Low, Medium, or High) and to create a predictive model using a Random Forest Tree Classifier to categorize stress levels based on their lifestyle habits and coffee consumption. 

Questions 
- Can lifestyle factors such as coffee intake, sleep hours, physical activity, age, and BMI accurately predict a person's stress level?
- Which features are most influential in determining stress levels?

## THE DATASET
The data I chose to use is a file found from Kaggle called https://www.kaggle.com/datasets/uom190346a/global-coffee-health-dataset.
My target variable is Stress_Level, and my main predictors would be Coffee_Intake, Caffeine_mg, Sleep_Hours, Sleep_Quality, Age, and BMI.

## PREPROCESSING
Some steps I took for preprocessing my data were to:
- Dealing with Non-Existent Data - Doing this step allowed me to use data that was relevant and existed to answer my questions and focus on columns that will contribute to my predictions. For this case, I removed a column as there was no information in it.
- Used Label Encoding - This step allows to convert labels I had in text form, that were Low, Medium, High, into a numerical format like 0, 1, 2 so the Random Forest Classifier could be able to process them.
- Used One Hot Encoding - Doing this step allowed all the columns to turn text categories into numbers that the Random Forest model can use, which is usually binary.
- Data Split: -  This allowed me to train the Random Forest model with a training set that was 80% and a testing set that was also 20%. This allows it to deal with unseen data, to get a measure of how well the model truly understood the relationships between lifestyle habits and stress models

## VISUALIZATION/DATA UNDERSTANDING
To explore this data, I plan to use a Random Forest Model. I have used Countplot, Bar Plots, ScatterPlot, and HeatMap


## MODELING


## EVALUATION


## STORY



## IMPACT


## REFERENCES
- This project was used using Jupyter Notebooks and was coded in Python with libraries such as Pandas, Matplotlib, Seaborn, and Scikit.
- The dataset used was [Global Coffee Health Dataset](https://www.kaggle.com/datasets/uom190346a/global-coffee-health-dataset) and the overall structure of this project should be
  *  `PROJECT2.ipynb`: My main code that has the data preprocessing, analysis, and visualization information.
 `https://www.kaggle.com/datasets/uom190346a/global-coffee-health-dataset.csv`: The raw dataset file.

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





