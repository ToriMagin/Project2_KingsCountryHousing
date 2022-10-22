# Project2_KingsCountryHousing

# Overview & Business Problem 

The client, a mid-size local real estate agency, needs data insights to advise homeowners and/or investors which house features and what type of renovations might increase house values.

To provide these insights, the King County Housing Data Set was analysed, which contains 20 features of houses sold in King County. A full description of the dataset's columns can be found below. The aim of this project is to develop a multiple regression model than can predict a house's price as accurately as possible.

# Data Understanding & Preparation
This dataset contains over 20,000 house sales from May 2014 to May 2015 for King County. The data represents 20 different house features and the sale price.

####  King County Data Set Columns
* id - unique identified for a house
* dateDate - house was sold
* price - is prediction target
* bedroomsNumber - of Bedrooms/House
* bathroomsNumber - of bathrooms/bedrooms
* sqft_livingsquare - footage of the home
* sqft_lotsquare - footage of the lot
* floorsTotal - floors (levels) in house
* waterfront - House which has a view to a waterfront
* view - Has been viewed
* condition - How good the condition is ( Overall )
* grade - overall grade given to the housing unit, based on King County grading system
* sqft_above - square footage of house apart from basement
* sqft_basement - square footage of the basement
* yr_built - Built Year
* yr_renovated - Year when house was renovated
* zipcode - zip
* lat - Latitude coordinate
* long - Longitude coordinate
* sqft_living15 - The square footage of interior housing living space for the nearest 15 neighbors
* sqft_lot15 - The square footage of the land lots of the nearest 15 neighbors


The target variable will be the sale price of the home, as the goal is to build a model to predict price. We selected features related to the house as the important predictor features.


Variables ID, date, latitude, longitude, and zipcode we’re removed as they were not considered reasonable predictors.


### Grouping 

Certain features were grouped to make them eaier to analyse wuithin the model. 

* **Year Renovated** was grouped into "Renovated - Yes" and "Renovated - No" as over 80% of the entries were not renovated and the remaining were thinly scatter over many years.  

* **Year Built** was grouped into four 30 year periods. 

* **Grade** was consolidated from 11 to 6 groups with quanlative names. 



