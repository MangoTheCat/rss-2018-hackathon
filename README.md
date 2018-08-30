# RSS 2018 Data Science Hackathon

This repository holds all material for the hackathon event at the RSS Conference 2018.

## Introduction

In this Hackathon hosted by Mango Solutions for the RSS, we want to help demystify what it means to do data science ‘in the wild’ by providing an opportunity to work with open data sets on a challenging problem.

The topic for the Hackathon is UK politics, with the data kindly provided by the hard efforts of [https://github.com/six50](https://github.com/six50).

We will be looking at past data on peoples voting patterns and demographics in order to have a go at two main tasks:

1. Visualising election results and other data across constituencies on a geographic map. 
2. Building models and predicting turnout at general elections using past results and polling data. 

In addition, both of these tasks will require an amount of data prep and manipulation to get to the end result. Examples are provided in this repository in both the R and Python programming languages (though you are free to use you own tools of choice as well!). Participants are encourages to go through these to build familiarity with the data and then build upon them with there own ideas for improvement. 


## Prerequisites

* If you are using Python, make sure you have the Anaconda Python distribution installed for Python 3.6. It can be downloaded from [https://www.anaconda.com/download/](https://www.anaconda.com/download/).

* If you are using R, make sure you have recent version of R and Rstudio installed. R can be downloaded from [https://cran.r-project.org/](https://cran.r-project.org/), and Rstudio from [https://www.rstudio.com/products/rstudio/download/](https://www.rstudio.com/products/rstudio/download/).

## Quick Start

1. Clone or download this repository.

2. Extract the data. The data folder contains zip files for each set of data. Unzipping them inplace will create the necessary folder structure for the examples. 

3. Install dependencies by following [setup-R.md](./setup-R.md) or [setup-Python.md](./setup-Python.md)

4. Either launch Rstudio (for R) or Jupyter Notebook (for Python) and navigate to the `examples/` directory. 

5. Step through the examples, gain intuition and extend!


# Task Details

## General Election Predictions

Two data sets are provided under `data/election`:

* `ge_2010_2015_training_data.csv` - Based on **2010 to 2015 General Election** plus polling data 3 days before election. 
* `ge_2015_2017_prediction_data.csv` - Based on **2015 to 2017 General Election** plus polling Data 3 days before election.

The task is to train a model on the first and use it to predict on the second. Full descriptions of the data fields are found under `data/Data-Description.md`.

The columns marked as missing, can be filled in by following the `Data-Pre-processing-Walkthrough-Election-Results` walkthrough in the examples. 

A basic model can be fit in by following the `Modeling-Walkthrough` in the examples. 

### Extension Ideas

* Look into Feature engineering and selection. 
    * Removing highly correlated variables?
    * Adding regional information?
    * Creating new features from the data?
    * You can add more data from other sources and build a completely different model

* Model Interpretation and Improvement
    * What constituencies/parties were predicted the best and worst?
    * Do other modelling approaches improve prediction?
    * How does your result compare to other forecasts for the election result?

* Anything else you can think of, be creative!


## General Election Result Visualisations

The `Election-Result-Visualisation-Walkthrough` goes through plotting the result of the 2010 election on a map of Wales, and shading the constituencies according to the party that won.


### Extension Ideas 

* Repeat with different regions and data sets:
    * Results for 2010 vs 2015 vs 2017
    * Scotland, England or all of UK

* Have a go at visualising the ['swing'](https://en.wikipedia.org/wiki/Swing_(United_Kingdom)) between different political parties.

* Add interactivity to th R example using the [mapview](https://github.com/r-spatial/mapview). See if you can overlay different years of results as layers on the map. 

* Add the prediction results from the modelling task and visualise them.

* Source other data sets and visualise how these vary by constituency. 

* Anything else you can think of, be creative!


# Collating Results

Results will be collated via a collaboratively edited google document as we go. Link to follow. 


# References

The following references may be useful to augment the analysis and visualisation tasks:

* [GE 2017 Datasets](http://bit.ly/UKPoliticsDatasets): – a crowdsourced collection of all kinds of relevant datasets.


