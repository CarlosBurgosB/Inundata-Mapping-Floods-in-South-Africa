# Inundata-Mapping-Floods-in-South-Africa
My solution to the Inundata: Mapping Floods in South Africa challenge by Zindi. The goal of the challenge was to predict flash floods from CHIRPS precipitation data and Sentinel 2 images.

Each time series has at most one flood event. As per the event organizers, probabilities cannot be threshold or rounded.

The Feature Engineering notebook has a small EDA and creates the necessary features for our prediction. Mainly lags, leads, and different rolling statistics. Also, for the images, vegetation indexes and Gray-Level Co-Occurrence Matrix features are calculated.

The Modelling notebook has the 10 fold cross validation using LightGBM for a model that predicts whether there's a flash flood event in a time series or not, and also for a model that predicts WHEN a flash flood might occur.

Submission notebook is not included since the challenge has already closed.
