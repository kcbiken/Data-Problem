# Data-Problem

![](https://raw.githubusercontent.com/UTA-DataScience/ProjectTempate/main/UTA-DataScience-Logo.png.png)

# Project Title: Sentiment Analysis of Stocks in reddit community (Wallstreet Bets)

* **One Sentence Summary** This repository holds an attempt to extract stocks' sentiments and insightful plots from the tiitles of the text collected from the post of user in WallstreetBets community.
*https://www.reddit.com/r/wallstreetbets/ 

## Overview

* This section could contain a short paragraph which include the following:
  * **Definition of the tasks / challenge** 
  * The main task of the project to find the sentiment of the stock mentioned on WallstreetBets and perform some additional  insightful visualization

  * **Your approach**
  * The approach in this repository formulates the task as Natural Language Processing task, using NLTK Vader which is one of the popular unsupervised machine learning algorithm. I have perfomed the task in two steps using two different python file i.e. Part1 and Part2. 
  * Part1.py will take the title of the user's post as an input for the model. The model will generate the sentiments based on the name of the stock. In addition, the model will generate the number of mentions of that stock within the given time frame. It then merges every dataframe together and save that as a csv file. Furthermore, this file also visualize some insightful comparision plots of the stock based upon the number of mentions and sentiments of the stock. 

  * Part2.py will take the above well merged dataframe as an input. Based upon the name of the stock this model will generate three insightful plots i.e. number of mentions of stock every week, sentiment of stock every week, and price of stocks every week. 
 
  * **Summary of the performance achieved**
The model is able to calculate the sentiment of stocks that are mentioned on WallstreetBets community on weekly basis. Also, it is able to count the number of times the stock has been mentioned on weekly basis. Based on those data, insightful visualization plots has been achived. 
 

## Summary of Workdone

Include only the sections that are relevant an appropriate.

### Data

* Data:
  * Type: For example
    * Input: raw text data from the title of the user's post
  * Size: weekly data
  * Instances: On average 4,000 data points every week

#### Preprocessing / Clean up

The raw text data from the title of the user's post may or may not contain the name of the stock. Only the tiltle that contains the name of the stock is selected as the input of the model. Those title were stored in dictionary categorized on the basis of the stock's name. Similarly, a dictionary of count of those stocks is created



### Problem Formulation

* Define:
  * Input / Output:
  Raw text data as input, insightful visualization plots as output
  * Models
  This problem is a Natural Language Processing Problem. Also, this problem is itself an unsupervised problem where there is no target label. Hence, NLTK Vader, one of the popular Natural Language Processing Technique, is a good pre-trained model to use for our problem. 

### Training
Since unsupervised model or model based on vocabulary is used, so training is not required for the model. Instead, the model is made robust by adding new list of words that are popular in stock market's conversation.

### Performance Comparison

* The key performance metric(s) in this project will be the dependency price of the stock with its sentiment.
* For every stock we can compare its price plot and its sentiment and make calculated guess on the future.
* <img width="639" alt="image" src="https://user-images.githubusercontent.com/89658256/166380730-5c82781f-a8d4-424c-adcf-5dc00350e883.png">
* <img width="628" alt="image" src="https://user-images.githubusercontent.com/89658256/166382948-49713945-0386-480c-b874-d33b2371a67e.png">


### Conclusions

* Some sentiment may correlate to the price of the stock but no direct correlation is found between the price of the stock and the calculated sentiment of the stock.  

### Future Work

* In future, I would like to find the correlation of stock and its sentiment not only on a weekly basis but also on daily, biweekly and monthly basis. 
* What are some other studies that can be done starting from here.

## How to reproduce results

* In this section, provide instructions at least one of the following:
   * Reproduce your results fully, including training.
   * Apply this package to other data. For example, how to use the model you trained.
   * Use this package to perform their own study.
   * To work with this package, first the user need raw weekly text data from reddit community (Wallstreetbets). 
* The package can be easily run on simple local computer. 

### Overview of files in repository

* Describe the directory structure, if any.
* Raw files: It contains the raw text dataset from reddit
* Insightful Dataset: It contains the dataset after preprocessing and modeling. It contains price, number of mentions and sentiment of stocks. 
* Reddit Sentiment Analysis Part 1.ipynb: This package will convert raw files to insightful dataset
* Reddit Sentiment Analysis Part 2.ipynb: This package will produce insightful plot from insightful dataset

* List all relavent files and describe their role in the package.
* An example:
  * utils.py: various functions that are used in cleaning and visualizing data.
  * preprocess.ipynb: Takes input data in CSV and writes out data frame after cleanup.
  * visualization.ipynb: Creates various visualizations of the data.
  * models.py: Contains functions that build the various models.
  * training-model-1.ipynb: Trains the first model and saves model during training.
  * training-model-2.ipynb: Trains the second model and saves model during training.
  * training-model-3.ipynb: Trains the third model and saves model during training.
  * performance.ipynb: loads multiple trained models and compares results.
  * inference.ipynb: loads a trained model and applies it to test data to create kaggle submission.

* Note that all of these notebooks should contain enough text for someone to understand what is happening.

### Software Setup
* List all of the required packages.
* Packages used: Pandas, Matplotlib, seaborn, request, yahoo finance, regular expression, pandas_datareader, nltk
* Any packages or libraries can be installed using the command "pip install package_name". For instance, pip install yfinance will install the package yahoo finance. 
* If not standard, provide or point to instruction for installing the packages.
* Describe how to install your package.

### Data

* Point to where they can download the data.
* Data can be download from this python code. Minor changes on date range is required to get the dataset within specific time interval.
* https://github.com/ahy3nz/ahy3nz.github.io/blob/master/files/notebooks/2021-02-01-reddit1.ipynb
* Lead them through preprocessing steps, if necessary.


## Citations

* Provide any references.
* https://github.com/ahy3nz/ahy3nz.github.io/blob/master/files/notebooks/2021-02-01-reddit1.ipynb
* https://github.com/jklepatch/eattheblocks/blob/master/screencast/290-wallstreetbets-sentiment-analysis/reddit-sentiment-analysis.py












