## Car Price Prediction

Hello Everyone,

Here is My Project which is executed during the internship in HexNBit based on Predicting Price of Car using Linear Regression.

## Dataset

I used Honda Used Car Selling Dataset which is one of Dataset uploaded on Kaggle.

**Link to the Dataset :** [Honda Used Car Selling](https://www.kaggle.com/datasets/themrityunjaypathak/honda-car-selling)

## Problem Statement

- The objective of this Project is to develop a Machine Learning Model that can accurately predict the prices of used cars based on various features and attributes.
  
- The predicted prices will assist both buyers and sellers in making informed decisions, ensuring fair transactions in the used car market.

## Table of Contents

- [Setting up the Enviroment](#setting-up-the-enviroment)
- [Libraries required for the Project](#libraries-required-for-the-project)
- [Getting started with Repository](#getting-started)
- [Steps involved in the Project](#steps-involved-in-the-project)
- [Conclusion](#conclusion)
- [Link to the Notebook](#link-to-the-notebook)

## Setting up the Enviroment

Jupyter Notebook is required for this project and you can install and set it up in the terminal.

- Install the Notebook - `pip install notebook`

- Run the Notebook - `jupyter notebook`

## Libraries required for the Project

**NumPy**

- Go to Terminal and run this code - `pip install numpy`

- Go to Jupyter Notebook and run this code from a cell - `!pip install numpy`

**Pandas**

- Go to Terminal and run this code - `pip install pandas`

- Go to Jupyter Notebook and run this code from a cell - `!pip install pandas`

**Matplotlib**

- Go to Terminal and run this code - `pip install matplotlib`

- Go to Jupyter Notebook and run this code from a cell - `!pip install matplotlib`

**Seaborn**

- Go to Terminal and run this code - `pip install seaborn`

- Go to Jupyter Notebook and run this code from a cell - `!pip install seaborn`

**Sklearn**

- Go to Terminal and run this code - `pip install sklearn`

- Go to Jupyter Notebook and run this code from a cell - `!pip install sklearn`

## Getting Started

- Clone the repository to your local machine using the following command :
```
git clone https://github.com/MasterMindRomii/Car-Price-Prediction-Model.git
```

## Steps involved in the Project

**Data Cleaning**

- Fuel Type, Suspension and Car Model has extra whitespaces which is removed by str.strip() Method.

- Removing kms Suffix from kms Driven Column by using str.split() Method and keeping only Numeric Part of the String and removing kms Suffix.

- After that we can convert kms Driven Column to int DataType.

- Modifying Price Column from 6.45 Lakh to 645000 and convering it into Integer by using a Custom Made Function.

- From Car Model Column we will keep only First 3 Words of Cae Model and removing the rest of the Words for better Model Traning.

**Data Visualization**

- Visualizing Year with Price by using sns.swarmplot().

- Visualizing kms Driven with Price by using sns.relplot().

- Visualizing Car Model with Price by using sns.relplot() and Suspension as Hue Parameter.

**Dummy Variable**

- We first Create Dummy Variable Column based on the Text Column.

- Then we change it into a DataFrame.

- After that we will Merge the Dummies DataFrame and our Orignal DataFrame.

- Finally we will drop the Text Column from our Dataset.

**Outlier Removal**

- After describing the Dataset I noticed that in our kms Driven Column, 75% of Cars has driven 85000 kms and our Maximum Value in kms Driven is 11 Lakh kms which is an Outlier.
  
- And Similarly In our Price Column, 75% of Cars has Price 7 Lakh and our Maximum Price is 26 Lakh which is an Outlier.

**Model Building**

- Firstly I have definied Dependent and Independent Variables for our Traning and Testing.

- I have splitted data into Traning and Testing Set by using Train Test Split.

- Then I fitted the Model with X_train and y_train and checked the Score.

- After that I used KFold Cross Validation for Measuring Accuracy of our Model.

- So I cheked Cross_Val_Score of our Model for Measuring the Best Score of Model and then I have taken Mean of All that Scores.

- And Finally I predicted the Result from our Trained Model.

## Conclusion

- Developed a highly accurate Linear Regression Model using various features and attributes to predict used car prices, achieving an average prediction accuracy of 82%.

- Further Model showcased its robustness by undergoing rigorous k-fold cross-validation, resulting in a mean cross-validation score of 83%.

## Thank you :)
