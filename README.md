## Amazon Reviews Proposal

Introduction
============

In this project, we collected people textual reviews about different purchased products from Amazon. the data set contains approximately 413,000 customer reviews including products prices, final customer ratings and the products' names.


Research Question(s)
====================

- What are the customers' sentiments for different products or brands based on their textual reviews ?

- Can we use the customers' textual reviews to predict the customers' sentiments ?

- Can we predict the customer ratings based on the given textual reviews and the price of the product ?




Approach
========

We are going to follow the steps below in order to systematically answer the research questions posed in `Research Question(s)` section above.

- We will use Natural Language Processing (NLP) methods and techiques to preprocess the textual data and convert them into suitable numerical formats compatible with different machine learning algorithms.

- We will use the processed data to computationally calculate the sentiment of the customer to a product.

- We will use the processed data to calculate the similarity between customers' reviews and predict sentiments for future reviews using classification models.


Data Description
================

- We used publicly available data set from KAGGLE website for Amazon Customer reviews.
- The data set contains approximately 413,000 Records, with initial 6 features/columns. The following table shows the general layout of the first few records.

|Product Name                                                                                             |Brand Name|Price |Rating|Reviews                                                                                                                                                                                                                                                                                                                                                                               |Review Votes|
|---------------------------------------------------------------------------------------------------------|----------|------|------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------|
|"CLEAR CLEAN ESN" Sprint EPIC 4G Galaxy SPH-D700*FRONT CAMERA*ANDROID*SLIDER*QWERTY KEYBOARD*TOUCH SCREEN|Samsung   |199.99|5     |I feel so LUCKY to have found this used (phone to us & not used hard at all), phone on line from someone who upgraded and sold this one. My Son liked his old one that finally fell apart after 2.5+ years and didn't want an upgrade!! Thank you Seller, we really appreciate it & your honesty re: said used phone.I recommend this seller very highly & would but from them again!!|1           |
|"CLEAR CLEAN ESN" Sprint EPIC 4G Galaxy SPH-D700*FRONT CAMERA*ANDROID*SLIDER*QWERTY KEYBOARD*TOUCH SCREEN|Samsung   |199.99|4     |nice phone, nice up grade from my pantach revue. Very clean set up and easy set up. never had an android phone but they are fantastic to say the least. perfect size for surfing and social media. great phone samsung                                                                                                                                                                |0           |
|"CLEAR CLEAN ESN" Sprint EPIC 4G Galaxy SPH-D700*FRONT CAMERA*ANDROID*SLIDER*QWERTY KEYBOARD*TOUCH SCREEN|Samsung   |199.99|5     |Very pleased                                                                                                                                                                                                                                                                                                                                                                          |0           |


Resources
=========

- KAGGLE Website <a href="http://www.kaggle.com">Go To KAGGLE</a>

- Data Set Direct Download, To download directly the data set please <a href="https://www.kaggle.com/nehasontakke/amazon-unlocked-mobilecsv"> Click here</a>


Tools and Libraries
===================

- Jupyter notebook
- Python 
- Scikit-Learn
- Spacy
- NLTK
- Pandas
- numpy
- Scipy
- Plotly



