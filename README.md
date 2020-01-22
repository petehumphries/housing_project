# Module 1 - Housing Project

## Executive Summary:

The goal of the project was to create a model that would determine the price of a property based on its attributes, with 
hopes that this will improve the time taken to sell. The project began by asking the question of how does
price change with distance from Downtown Seattle. The coordinates of each house and Downtown Seattle seattle were used
to calculate a distance. A strong negative correlation could be seen between the two variables. Next, it
was determined which variables could best predict the price of a house. These were found to be the the following:

1. Square feet of living space.
2. Number of views the property has had. 
3. Whether or not the property was on the waterfront.
4. Distance to Downtown Seattle.

A multivariate linear regression analysis was conducted with these variables to get a line of best fit, from which the 
price of a house can be determined. Finally, it was found that separating the dataset into individual zipcodes yielded 
a 6% improvement in the fit of the model. This is likely due to house attributes having different desirability in 
different areas.
 
## To keep the workflow clear this project was split into two notebooks:

1. Preprocessing 
2. Analysis

### Preprocessing

The purpose of the preprocessing stage is to ensure that a fully augmented and cleaned dataset is prepared before 
the start of the regression analysis stage. The aim is to ensure that all data cleaning takes place upstream. The notebook
was constructed as follows:

1. Import the libraries required in the analysis / active workbooks (Pandas, NumPy, Matplotlib, Seaborn, maths, statsmodel).
2. Import raw data file KC Seattle Housing Data Set containing descriptive variables of houses sold in 2014-2015 and sales 
prices.
3. Creating new columns for new or transformed data (including distance calculations). 
4. Data familiarisation, cleansing and treatment. 
5. Removal of duplicates.
6. Standardisation.
7. Save down a cleaned data CSV to be used in regression analysis sheet. 

### Analysis

The Analysis stage takes the cleaned and augmented data set as the only input to the process.In the analysis phase 
data visualisations, correlation matrices, maps, univariate regressions and multivariate regressions are used to get 
a feel for the dataset.

1. Import python libraries and the cleaned data .csv file. 
2. Plot a correlation matrix.
3. Linear regression.
4. Multi-variate regression. 
5. Data visualisation.
6. Outlier treatment.
7. Zipcode analysis.
