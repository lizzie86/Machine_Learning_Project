

# Predicting Land Acquisition Cost and Forest Change in Massachusetts

This project is a geospatial analysis of predicting land acquisition cost and forest change across 177,277 parcels in Massachusetts using various machine learning methods( Linear Regression, Gradient Boosting, Random Forest, Extremely Randomized Trees, K-fold cross-validation, Out-Of-Bag Estimate). The document provides insights on how to prepare the data (pandas, numpy, geopandas), create the maps of predicted values and residuals(matplotlib), and how to build machine learning models with geodataframe (statsmodels and scikit-learn).

## Data
- The parcel dataset, including the last sale data and the parcel ID ('pid'), is an extract from PLACES(the Private-Land Conservation Evidence System)(placeslab.org/places).
- The underlying vector data, all parcels in Massachusetts that are larger than one hectare (nobs = 220,187), comes from the Standardized Assessor's Parcels provided by MassGIS.
  https://www.mass.gov/info-details/massgis-data-property-tax-parcels

## Contents

The ipynb file contains the following information:

1. Data Preprocessing: 
- How to use the parcel ID(pid) to join shapefile and other data for analysis
- Details on the process of creating a Geodataframe of parcel centroids and its significance in the analysis
- Creating outcome and independent variables for the analysis
- Create the data frame for the analysis

2. Predicting land acquisition cost: Predictive modeling with k-fold cross-validation (k=5)
- Simple Linear regressions
- Linear Regression model 2: Remove the time trend
- Linear Regression model 3: add quadratic and interaction terms
- Ensemble Methods: Gradient Boosting, Random Forest, Extremely Randomized Trees
3. Tree Models with Out-Of-Bag (OOB) Estimate
4. Adding x and y coordinates of each parcel to incorporate variations across space,
4. Find well-performing models based on out-of-sample error
5. Predicting forest cover change across Massachusetts with the best model we found above


## Usage

This repository is for reference purposes only and is not open for contributions. The information provided in the document can be used to gain insights into geospatial analysis and predictive modeling for land acquisition and forest change. 

