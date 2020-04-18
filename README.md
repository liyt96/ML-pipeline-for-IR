# ML-pipeline-for-IR

### Introduction

A Machine Learning pipeline for Information Retrieval.

### Feature Engineering

The Machine Learning model takes 5 IR scores: 
* Okapi TF
* TF IDF
* BM 25
* Unigram LM with Laplace smoothing
* Unigram LM Unigram LM with Jelinek-Mercer smoothing 

as features. The scores are calculated by the documents and the query.

### Why Linear Regression?

The model fits on a [Linear Regression](https://en.wikipedia.org/wiki/Linear_regression) algorithm.

We may infer that, the higher the IR scores, the more likely a document is relevant to a user's query. Thus the features (5 IR scores) and the prediction (predicted score) should be linear dependent, and a linear model like linear regression should be good to express their relationship.
