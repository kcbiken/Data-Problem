# Data-Problem

Function:

Part1 file: a)convert raw text data into the dataframe of count of mentions and sentiment of stock
            b)convert those dataframe into csv file and save it

Part2 file: a)use the above dataframe stored in csv file to visualize various insightful plots

![](https://raw.githubusercontent.com/UTA-DataScience/ProjectTempate/main/UTA-DataScience-Logo.png.png)

# Project Title: Sentiment Analysis of Stocks in reddit community (Wallstreet Bets)

* **One Sentence Summary** This repository holds an attempt to extract insightful plots from the tiitles of the text collected from the post of user in WallstreetBets community.
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
  * The model is able to calculate the sentiment of stocks that are mentioned on WallstreetBets community on weekly basis. Also, it is able to count the number of times the stock has been mentioned on weekly basis. Based on those data, insightful visualization plots has been achived. 
 

## Summary of Workdone

Include only the sections that are relevant an appropriate.

### Data

* Data:
  * Type: For example
    * Input: raw text data from the title of the user's post
  * Size: weekly data
  * Instances: On average 4,000 data points every week

#### Preprocessing / Clean up

* Describe any manipulations you performed to the data.
* The raw text data from the title of the user's post may or may not contain the name of the stock. Only the tiltle that contains the name of the stock is selected as the input of the model. Those title were stored in dictionary categorized on the basis of the stock's name. Similarly, a dictionary of count of those stocks is created

#### Data Visualization

Show a few visualization of the data and say a few words about what you see.

### Problem Formulation

* Define:
  * Input / Output
  * Raw text data as input, insightful visualization plots as output
  * Models
    * This problem is a Natural Language Processing Problem. Also, this problem is itself an unsupervised problem where there is no target label. Hence, NLTK Vader, one of the popular Natural Language Processing Technique, is a good pre-trained model to use for our problem. 
  * Loss, Optimizer, other Hyperparameters.

### Training

* Describe the training:
  * How you trained: software and hardware.
  * How did training take.
  * Training curves (loss vs epoch for test/train).
  * How did you decide to stop training.
  * Any difficulties? How did you resolve them?

### Performance Comparison

* The key performance metric(s) in this project will be the dependency price of the stock with its sentiment.
* For every stock we can compare its price plot and its sentiment and make calculated guess on the future.
* <img width="639" alt="image" src="https://user-images.githubusercontent.com/89658256/166380730-5c82781f-a8d4-424c-adcf-5dc00350e883.png">
* <img width="628" alt="image" src="https://user-images.githubusercontent.com/89658256/166382948-49713945-0386-480c-b874-d33b2371a67e.png">


### Conclusions

* State any conclusions you can infer from your work. Example: LSTM work better than GRU.

### Future Work

* What would be the next thing that you would try.
* What are some other studies that can be done starting from here.

## How to reproduce results

* In this section, provide instructions at least one of the following:
   * Reproduce your results fully, including training.
   * Apply this package to other data. For example, how to use the model you trained.
   * Use this package to perform their own study.
* Also describe what resources to use for this package, if appropirate. For example, point them to Collab and TPUs.

### Overview of files in repository

* Describe the directory structure, if any.
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
* If not standard, provide or point to instruction for installing the packages.
* Describe how to install your package.

### Data

* Point to where they can download the data.
* Lead them through preprocessing steps, if necessary.

### Training

* Describe how to train the model

#### Performance Evaluation

* Describe how to run the performance evaluation.


## Citations

* Provide any references.






