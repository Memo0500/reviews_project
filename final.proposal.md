
## Amazon Reviews MVP

Introduction
============

In this project, we collected people textual reviews about different purchased products from Amazon. the data set contains approximately 413,000 customer reviews including products prices, final customer ratings and the products' names.


Approach
========

We are going to follow the steps below in order to systematically answer the research questions posed in `Research Question(s)` section above.

- We will use Natural Language Processing (NLP) methods and techiques to preprocess the textual data and convert them into suitable numerical formats compatible with different machine learning algorithms.

- We will use the processed data to computationally calculate the sentiment of the customer to a product.

- We will use the processed data to calculate the similarity between customers' reviews and predict sentiments for future reviews using classification models.

- We will apply PCA-SVD techniques in order to reduce the dimensions of the data and improve the prediction through utilizing the latent dimensions discovered by those methods.

- Moreover, we will apply Non negative Matrix Factorization (NMF) and Linear Semantic Analysis (LSA) on smaller data set to diagnose any problems. Afterwards, we will implement Linear Discriminant Analysis (LSA) on the whole data set.

- We will perform Topic Modeling on negative and positive sentiments separately.

<img src="1.png">

<img src="2.png">


Data Description
================

- We used publicly available data set from KAGGLE website for Amazon Customer reviews.
- The data set contains approximately 413,000 Records, with initial 6 features/columns. The following table shows the general layout of the first few records.

Objectives
==========

- Using unsupervised machine learning techniques along with NLP methods to understand customers’ sentiments over different products.
- Explain the differences between customers’ reviews based on latent topics contained within to better tailor future marketing and product improvements.


Results
=======

- We utilized unsupervised machine learning techniques to gain more insights into mobile products reviews of amazon.
- The dataset contains approximately 417000 records which explain customers’ ratings , sentiments and reviews over a set of predefined mobile products

1. ### Data Understanding

<img src="3.png">
<br/>

<img src="4.png">
<br/>

<img src="best.five.png">
<br/>

<img src="positive.elbow.png">
<br/>

<img src="negative.elbow.png">
<br/>


2. ### Clustering 

- By performing clustering on positive reviews and negative reviews separately, we found unequal latent dimensions between these two categories.
- Positive reviews can be represented sufficiently by only two latent dimensions whereas negative reviews could be represented by more than two latent dimensions with very low overlap.



<img src="kmeans1.png">
Five Latent Topics for positive reviews
<br/>

<img src="kmeans2.png">
Two Latent Topics for positive reviews
<br/>


<img src="kmeans.2.negative.png">
Two Latent Topics for negative reviews
<br/>

<img src="scatter.text.png">
Scatter Text for positive vs negative reviews
<br/>

3. ### Classification on Vectorized Text

|Logistic regression|Accuracy|precision|Recall|F1-score|Logistic regression|Accuracy|precision|Recall|F1-score|
|-------------------|--------|---------|------|--------|-------------------|--------|---------|------|--------|
|Train              |0.76    |0.8      |0.79  |0.79    |Train              |0.805   |0.813    |0.821 |0.829   |
|Val                |0.69    |0.69     |0.69  |0.68    |Val                |0.68    |0.677    |0.674 |0.671   |
|Train-no noise     |0.76    |0.77     |0.76  |0.76    |Train-no noise     |0.76    |0.759    |0.758 |0.757   |
|Val –no noise      |0.68    |0.68     |0.68  |0.67    |Val –no noise      |0.67    |0.667    |0.664 |0.661   |
|Train-ngrams       |0.85    |0.86     |0.85  |0.85    |Train-ngrams       |0.85    |0.849    |0.848 |0.847   |
|Val-ngrams         |0.71    |0.72     |0.71  |0.71    |Val-ngrams         |0.71    |0.709    |0.708 |0.707   |
|Train-Trigrams     |0.86    |0.87     |0.86  |0.86    |Train-Trigrams     |0.86    |0.859    |0.858 |0.857   |
|Val-Trigrams       |0.72    |0.72     |0.72  |0.71    |Val-Trigrams       |0.71    |0.707    |0.704 |0.701   |



|SGB Classifier|Accuracy|precision|Recall|F1-score|
|--------------|--------|---------|------|--------|
|Train         |0.74    |0.75     |0.74  |0.73    |
|Val           |0.67    |0.67     |0.67  |0.66    |
|Train-no noise|0.71    |0.73     |0.71  |0.7     |
|Val-no noise  |0.64    |0.65     |0.64  |0.63    |
|Train -ngrams |0.69    |0.71     |0.69  |0.68    |
|Val-ngrams    |0.69    |0.64     |0.64  |0.63    |
|Train-unigrams|0.79    |0.81     |0.79  |0.79    |
|Val-unigrams  |0.69    |0.7      |0.69  |0.68    |



Future Work
===========

- Enhancing machine learning pipeline for better NLP text processing.
- Trying stacking classifiers and ensemble classifiers on reduced NLP dataset.






