# Sentiment Analysis on Movie Reviews

## Introduction
Build an end-to-end sentiment classification system from scratch. The system accepts a movie review as input and classifies it as either positive or negative. There are three main steps:

* Preprocess the data - Split the data into train and test sets, tokenize, stem words, create bag-of-words features, etc.
* Models - Create and experiment with different models: GaussianNB, Gradient-Boosted Decision Tree classifier and Recurrent Neural Network.
* Evaluation - Compare the performances of the models and outline steps to make the chosen model do better.

## Code

* `sentiment_analysis.ipynb` - Main code for sentiment analysis.
* `text_processing.ipynb` - Exampe code on how to preprocess data.

## Setup

* Python 3.6+
* The packages mentioned in `requirements.txt`. They can be installed using:

  `pip install -r requirements.txt`

## Data

* Data files for the sentiment analysis project are included under `data/imdb-reviews`. These are movie reviews from the website [imdb.com](https://www.imdb.com/), each labeled as either 'positive', if the reviewer enjoyed the film, or 'negative' otherwise. 
* These files take a while to load. To save time from reading them in everytime I run the notebook, I have created `data.pickle` and `labels.pickle` in the Explore step in `sentiment_analysis.ipynb`. As long as these pickle files are present in the same directory, I don't have to read in the review files from scratch.
* The rest of the data files in `data/` are for `text_processing.ipynb`.
* Some of the NLP libraries require additional data for performing tasks like stopwords, PoS tagging, lemmatization, etc. Specifically, `nltk` will throw an error if the required data is not installed. You can use the following Python statement (in Linux terminal or in a code editor) to open the NLTK downloader and select the desired package(s) to install:

  `nltk.download()`

  You can also download all available NLTK data packages, which includes a number of sample corpora as well, but that may take a while (10+GB).

## Run

To run any script file, use:

`python <script.py>`

To open a notebook, use:

`jupyter notebook <notebook.ipynb>`

