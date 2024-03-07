# Titanic survival prediction
This project is an introduction to a simple classification problem using the titanic dataset from Kaggle. The goal of this model is to predict if a passenger would have survived the titanic disaster

## Technologies used
- Python 3.10
- Anaconda
- Scikit-learn
- Pandas

## Learning outcomes
### Studying the dataset
  - better understand the datasets size, features and feature types
### Data Cleansing
  - handling missing data
### Feature engineering
  - **One-hot encoding** 
    - turning our categorical data into numerical data using `pandas` `get_dummies` method
    - taking a numerical class with multiple options and first studying how this feature could affect outcome then determining whether or not to apply the changes
  - **Binning** 
    - Taking another numerical class `Age` with the desire to avoid the model from using linear thinking to age by assessing the passenger being above or below a certain age leading to survival rate and utilizing binning to separate the feature into 10 buckets and applying one-shot encoding to create the new categorical features
  - **Feature Selection** 
    - Determine unecessary columns and remove them from our dataset
### Model Training
  - **Splitting data**
    - Apply a 60/20/20 Train/Val/Test data split
  - **Evaluate different models**
    - Review Logistic Regression, decision tree, naive Bayes, support vector machine, random forest, gradient boosted tree, and an AdaBoost Model
    - Evaluate F1 scores and overall accuracy of each model
  - **Hyperparameter Tuning**
    - Utilize Grid Search for our SVM model and apply the kernel trick with RBF (radial basis function)
    - Utilize k-fold cross validation

## Running/testing locally
This project utilizes Anaconda so as long as you have it installed locally you will need to activate the `titanic` environment located in `./environment.yml`
```
conda env create --file=environment.yml
conda activate titanic
```