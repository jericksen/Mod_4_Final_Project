# Module Four Final Project

For: Trace Political, LLC

By: Jonathan E. Ericksen, JE Consulting

## Background
> Trace Political is a consulting firm that specializes in social media consulting for congressional campaigns. Trace Political has contracted with JE Consulting to run an analysis on ~86K tweets from sitting congressional representatives. The tweets were acquired from May 2018 and are expected to yield valuable insights into the social media behavior and trends from current elected officials. 

## Objective:
The objective for JE Consulting is two fold: 

>- **Objective One: Corpus Analysis**

    - Extract the top 10 most words used within tweets from both Democrat and Republican representatives
    - Extract the total vocab count used in both the Democrat and Republican tweet corpus'
    - Extract words with the highest semantic relation to the following through word vectorization: 
        - Trump
        - Bill
        - Tax
    - Using TextBlob, extract the sentiment rating for Democrat and Republican tweets

>- **Objective Two: Tweet Classification using Neural Networks**

  > In addition to corpus analysis, Trace Political has asked JE Consulting to suss out the feasibility of building a classifier using neural networks that successfully predicts the political party of which the author of an official tweet belongs. In order to be deemed successful, the model must successfully predict political party with 90% accuracy on test data. Should this succeed, Trace Political will further pursue projects related to predictive modeling with natural language processing.
  
  >*Question:*
  > Can a neural network successfully classify political affiliation based on language contained in official tweets from the available dataset?

## Methodology:

> This project is broken down in to two parts. Part One will will address the first objective which is to perform basic analysis of the text corpus contained within tweets from the dataset. Part Two will attempt to model the text data resulting in successful party classification. Part Two will finish with a conclusion based upon the attempted modeling along with recommendations for future work to enhance model performances, et cetera. The sections and sub-sections are outlined in the table of contents below.

## Table of Contents:
### Obtain 
> - Sourcing the Data
> - Importing Data

### Part One

> - Exploratory Data Analysis 
> - Number of Tweets By Party
> - Common Words by Party
> - Vocab Length
> - Semantic Relationships
> - Sentiment Analysis

### Part Two

> - Feature Engineering
    
    - Data Cleaning
    - Convert Labels to Integers
    - Tokenize Text
    - Padding Input Matrices
    - Train Test Split
> - Modeling
    
    - LSTM Model One
    - LSTM Model Two
    - LSTM Model Three
    - GRU Model One
    
**Conclusions**

***Question:*** 

Can a model successfully classify political affiliation based on language contained in official tweets?

***Answer:*** 

Based on the objectives set forth by Trace Political, it seems we have failed to produce a model that can predict party affiliation with a 90% accuracy score. Further, each model exhibited clear signs of over fitting which does not lend itself to any succesful real world deployment of these models.

The short answer here as to why our models have failed is the simple fact that we are not operating with enough data. Future iterations of this objective would require additional web scraping to acquire enough tweets to improve the predictive power of our models. 

**Recommendations**

The models produced above exhibit clear over fitting on the training data. Further, the predictive power of each model downright abysmal to somewhat applicable. To combat this, we recommend acquiring further tweet data from which our models can learn. 

Additionally, Trace Political should look to data sources beyond twitter. Perhaps other forms of social media would provide rich data sets that can be used to train an NLP models. Perhaps facebook or even press releases might offer valuable data that unlocks keywords used in the language by party. 

**Future Work**

Future work is needed to further refine and tune both the hyperparameters of these models as well as the overall model architectures. Doing so would enforce the idea of needing more data. 

Additionally, further work could be done on practices used with cleaning the text data. It is likely there if predictive information stored within some of the symbols and characters commonly used within tweets outside of words. 

Finally, work should be done with to develop a relevant use case for a model that accurately predicts political party by tweet content. Though we did not meed Trace Political's threshold for deeming this project a success, with more data and model/data cleaning experimentation, a powerful model may still be possible. Once one is developed, ways to employ the model should be flushed out for use within Trace Political's product offering.
