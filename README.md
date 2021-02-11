# ML-pipeline-for-IR

### Introduction

A Machine Learning pipeline for Information Retrieval. Builds a machine learning based search engine for news articles.

### Feature Engineering

The Machine Learning model takes 5 Information Retrieval Scores: 
* Okapi TF
* TF IDF
* BM 25
* Unigram Language Model with Laplace smoothing
* Unigram Language Model with Jelinek-Mercer smoothing 

as *features*. The scores are calculated by the documents given the queries.

### Why Linear Regression?

The model fits on a [Linear Regression](https://en.wikipedia.org/wiki/Linear_regression) algorithm.

We may infer that, the higher the IR scores, the more likely a document is relevant to a query. Thus the features (5 IR scores) and the prediction (predicted score) should be linear dependent, and a linear model like linear regression should be good to express their relationship.
