# Titanic : Visualization & Prediction
Predict survival on the Titanic 
 -Sayudh Mukherjee.

<img src="https://wallpaperaccess.com/full/1161691.jpg" height="70%" width="80%" >


## Requirements

This project requires  **Python 3+**  and the following Python libraries installed:

-   [NumPy](http://www.numpy.org/)
-   [matplotlib](http://matplotlib.org/)
-   [seaborn](https://stanford.edu/~mwaskom/software/seaborn/#)
-   [scikit-learn](http://scikit-learn.org/stable/)
-   [XGBoost](https://xgboost.readthedocs.io/en/latest/)
-   [Pandas](https://pandas.pydata.org/)

You will also need to have the software installed to run and execute an  [iPython Notebook](http://ipython.org/notebook.html)

## Code

An ipython notebook is used for data preprocessing, feature transforming and outlier detecting. All core scripts are in `file .ipynb"` folder. All input data are in `input` folder and the detailed description of the data can be found in [Kaggle](https://www.kaggle.com/c/titanic/data).

## Key features of the model training process

K Fold Cross Validation: Using 5-fold cross-validation.

First Level Learning Model: On each run of cross-validation tried fitting following models :-
1. Random Forest classifier
2. Extra Trees classifier
3. AdaBoost classifer
4. Gradient Boosting classifer
5. Support Vector Machine

Second Level Learning Model : Trained a XGBClassifier using xgboost


## Content in Notebook
1.  Data Preprocessing
2.  Exploratory Visualization 
3.  Feature Engineering  
    1. Value Mapping  
    2. Simplification 
    3. Feature Selection  
    4. Handling Categorical Data
4.  Modeling & Evaluation
    1. Trying Different Model without Validation
    2. Cross-validation method 
    3. Model scoring function
    4. Setting Up Models
5.  Train & Fit Model
6.  Our Base First-Level Models
7.  Second-Level Predictions From The First-Level Output
8.  Output as Prediction file ( .csv)
9.  Acknowledgments

## FlowChart

<img src="https://github.com/Sayudh-git/Titanic-Prediction-ML/blob/main/fig/flowchart.png" height="70%" width="80%"
     title="FlowChart">


## Prediction & Submission

The modal comparison with cross validation for first output layer :
<img src="https://github.com/Sayudh-git/Titanic-Prediction-ML/blob/main/fig/model_comparison_with_validation.png"
     title="xgboost with validation" height="70%" width="80%">


The final price prediction for each house is present in the `output` folder as a .csv file. The final model used for scoring is hypertuned XGBoost Classifier with Cross Validation. 

The final XGBoost Classifier can be viewed as :
<img src="https://github.com/Sayudh-git/Titanic-Prediction-ML/blob/main/fig/xgboost_with_validation.png" height="70%" width="80%"
     title="xgboost with validation">

## Contributors
Sayudh Mukherjee

## Acknowledgments

Inspirations are drawn from various Kaggle notebooks but majorly motivation is from the following :

1. https://www.kaggle.com/arthurtok/0-808-with-simple-stacking
2. https://www.kaggle.com/usharengaraju/data-visualization-titanic-survival
3. https://www.kaggle.com/arthurtok/introduction-to-ensembling-stacking-in-python
4. https://www.kaggle.com/startupsci/titanic-data-science-solutions


