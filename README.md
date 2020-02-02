# Collaborative Filtering Recommender system

## I recommend using [Jupyter Nbviewer](https://nbviewer.jupyter.org/) to view this notebook as Plots aren't rendering in Github

## Introduction

In this notebook I'll build Recommender system using SVD (Singular value decomposition)<Br>
    I'll be using [Book-Crossing Dataset](http://www2.informatik.uni-freiburg.de/~cziegler/BX/) which has BX-Books, BX-Users and BX-Book-Ratings in CSV format<Br>
    I'll only be using BX-Books and BX-Book-Ratings to build Recommender system as BX-Users has User related data which I dont require in this model
    

Steps which are involved in building this Recommender system
* Preprocessing
    * Loading the data and adjusting the error lines in dataset
    * Scraping with BeautifulSoup and Requests to find Missing Authors and Publishing Years
    * Cleaning Text data using Regex
* EDA
    * Plotting Top rated books using Plotly's [Sunburst Chart](https://plot.ly/python/sunburst-charts/)
    * Plotting Books with Highest average rating using [Bar Chart](https://plot.ly/python/bar-charts/)
    * Plotting Count plot of Users who gave more ratings
* Matrix Factorization
    * Using Scipy's SVD and find the missing rating
* Recommender system
    * Building a function that recommends books which are read by other similar users
    * and Finally building a function which plots the images of books as recommendations
