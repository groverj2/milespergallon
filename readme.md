# Predict mileage of cars, given values of following parameters for around 400 cars
#### This project is a simple regression prediction problem to be solved by machine learning algorithms.
#### The mission is to predict the mileage of a particular car given data of following parameters (features) for hundreds of cars:

    1. mpg:           continuous
    2. cylinders:     multi-valued discrete
    3. displacement:  continuous
    4. horsepower:    continuous
    5. weight:        continuous
    6. acceleration:  continuous
    7. model year:    multi-valued discrete
    8. origin:        multi-valued discrete
    9. car name:      string (unique for each instance)

The data concerns city-cycle fuel consumption in miles per gallon, to be predicted in terms of 3 multivalued discrete and 5 continuous attributes

#### The steps I have followed are more or less commonly followed steps for all regression machine learning problems.
#### However, I have displayed and explained 2 other key aspects of approaching and solving a regression machine learning problem
1. using cross_val_score to choose the best ML algo
2. select features using backward elimination, one of the many techniques available for feature selection or feature reduction

Actually both points mentioned above are really not needed for this project since its a really simple prediction problem given only these limited number of features

## Steps followed and described in the jupyter notebook

### 1. Read data file using pandas read_csv()

### 2. Data preprocessing and visuallisation
- Check for null, missing, incomplete, inappropriate values
- Clean the data by converting data type to appropriate data types, filling missing values, normalising etc.

#### 2a. Plot - to check any anomaly, outlier, distribution, range of values etc,
- pairplot of dependent variable (y) with respect to every independent variable or feature (x1, x2, x3 etc)
- histogram of dependent variable (y) and every independent variable or feature (x1, x2, x3 etc)
- boxplot of every independent variable or feature (x1, x2, x3 etc) to see if any outliers

### 3. Set up X and y dataframes for dependent variable (y) and independent features (x1, x2, x3 etc)

#### 4. Coverting features to log since they are not normally distributed

#### 5. Onehotencoding / labelencoding not needed since all discrete (categorical) variables are already numercial

#### 6. Run Random forest machine learning algo


```python

```


```python

```

## Now, the following 2 items are the 2 other key aspects I mentioned earlier

### 1. How to select the best Machine Learning algo for this regression problem

> #### Using <font color="green">cross_val_score</font> and <font color="green">KFold</font> , test common ML regression algos and finalising on the best based on the estimator score

#### 2. Run backward elimination to select best features (feature selection)

> #### Feature Selection technique to reduce the number of features when there are hundreds or thousands of features.


```python

```
