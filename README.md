# Title

**Authors**: Suraj, Carlos Mccrum, Lenore Perconti

## Overview

Project Two for Flatiron Data Science BootCamp. In this Project we sift through the data to see what we find in the Seattle Housing Market. We start by importing neccassary packeges, cleaning the data and sticking to the significant variables to help us understand the market. We want to know what home features we would like to help our stakeholders get a better overall average price for homes sold. Some of our recomendations include, home rennovations, more square living space and a sticking to newer homes.

## Business Problem

Our Stakeholder are Real Estate agencies in King County, Washington. The year is 2016. Real Estate agencies want to stand out in the competitive Seattle Housing Market and learn what factors for homes lead to better than average sale prices to focus their listing efforts on those homes.

In the following project, we take a look at the King County House Data and find a linear regression model that allows us to make inferences on what factors will lead to a house selling for above the average home price.

## Data

The is from King County housing in Washington and spans home sales between 2014 and 2015. This Data can be sourced here: https://www.kaggle.com/shivachandel/kc-house-data. The dataset consisted of 21 variables and 21613 observations.

## Methods

We first explored the data to see the contents and determine the relevancy of each variable to our Business Problem. Then we ran a heatmap and looked at initial correlation statistics of each variable to Sale Price, our target. 

We then split the data into testing and training groups. With our training group we then cleaned the data, which included eliminating highly correlated variables, replacing NAN values, and transforming categorical data into useable 'dummy' variables.

We then ran a baseline model using only sale price. Building off this, we took our most highly correlated variable, `sqft_living` and ran a simple linear model. We then added more highly correlated variables to the model and found an ideal model of the following variables `sqft_living`, `bathrooms`, `is_rennovated`. 

We then created visuals for the presentation. 

## Results

The third model of the following variables `sqft_living`, `bathrooms`, `is_rennovated` returned an R Squared value of: 0.448

Our results may generalize beyond this data set, but we were only working with one year worth of data and would possibly need more observations to be able to make inferences beyond this dataset. 

## For More Information

Please review our full analysis in [our Jupyter Notebook](./Project.ipynb) or our [presentation](./PDF-HERE).

## Repository Structure

Describe the structure of your repository and its contents, for example:

├── README.md                           <- The top-level README for reviewers of this project, you are reading it right now. 
├── dsc-phase1-project-template.ipynb   <- Narrative documentation of analysis in Jupyter notebook using python
├── DPDF_HEREpdf         <- PDF version of project presentation
├── code
│   ├── __init__.py                     <- .py file that signals to python these folders contain packages
│   ├── visualizations.py               <- .py script to create finalized versions of visuals for project
│   ├── data_preparation.py             <- .py script used to pre-process and clean data
│   └── eda_notebook.ipynb              <- Notebook containing data exploration
├── data                                <- Both sourced externally and generated from code
└── images                              <- Both sourced externally and generated from code
