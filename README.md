# About this project

In this project, the author showcases the practical use of the following
data science capabilities:

-   Data collection from unstructured sources
-   Data cleaning & transformation
-   Data visualization
-   Statistical data analysis
-   Predictive machine learning models

## Contact information

-   This notebook was last updated on: 2023-03-07
-   Author:
-   Connect on LinkedIn:

## Data collection and cleaning

In this project, we scrape data from the
[BoligPortal](www.boligportal.dk) website, where we have multiple
dynamically updated web pages with various rental accommodations. As a
part of this process, we download data on all rentals in the Greater
Copenhagen and clean it up so that it can be used for analytical
purposes. The cleaned-up data is stored in the `Data` folder.

### Learn more about the data scraping and cleaning

For more information on the kind of data collected and the specifics of
the method used, please refer to the
`BoligPortal data scraping and prep.ipynb` notebook.

## Exploratory data analysis

After the data is sourced and cleaned, the actual analysis begins. At
this stage, we're only looking into inferential statistics, where we
explore various variables by looking at a series of different charts. It
is in this part that we get to know what data is available and how the
data looks like in practice.

In this part, we explore both continuous and categorical varibales. We
use histograms and boxplots to investigate the distribution of
continuous variables, while categorical variables are mostly explored
using pie charts and barplots. Some scatter plots are used to visualize
the correlation between categorical variables, while geolocation data is
plotted on a map.

### Learn more about the exploratory analysis

For more details, please refer to the
`BoligPortal exploratory analysis.ipynb` notebook.

## Statistical data analysis

The exploratory analysis has inspired a number of different hypotheses
that are being put to the test in the next stage of the project. Some
examples include:

-   Monthly rent is higher for accommodations with a bigger size
-   Monthly rent per square meter is higher in the city than it is in
    the suburbs
-   Monthly rent per square meter is decreasing as we get further away
    from the nearest metro and/or S-train station

These and other hypotheses are thus tested using multiple linear
regression analysis (OLS) and in most cases, we find clear evidence
either confirming or rejecting them.

### Learn more about the statistical analysis

For more details, please refer to the
`BoligPortal statistical analysis.ipynb` notebook.

## Predictive analysis

The statistical analysis is carried out with the purpose of getting an
understanding on how different factors such as size, location etc.
affect the prices of rental accommodations. However, even though model
fit is evaluated and commented on, the analysis doesn't focus on
maximizing predictive power or producing a more robust model that could
also be applied to data outside of the sample.

For these purposes, a separate predictive analysis is carried out, where
several different machine learning (ML) models are utilized (random
forest regression, to be specific). The data is split into `75:25`
training vs. test set so that the models are developed based on the
training data but evaluated based on how well they predict based on the
test data. In order to improve the predictive power, further data is
added and an automated parameters hypertuning is performed.

### Learn more about the predictive analysis

For more details, please refer to the
`BoligPortal predictive analysis.ipynb` notebook.
