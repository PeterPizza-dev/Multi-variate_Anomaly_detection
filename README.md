# Anomaly detection in multivariate timeseries

This project is carried out as a part of the 02456 Deep Learning course at The Technical University of Denmark(DTU). 

The project was carried out by: 
* Oliver Behrens, s163866
* Tue Thomsen, s163852
* Emil Lindegaard, s165016
* Stine Poulsen, s153609

### Abstract from research paper: 
This paper investigates anomaly detection in wooden structures using multivariate time series. The goal was, with no ground truth, to predict when anomalies occur using unsupervised learning methods. The performance of three different models was investigated: An auto-encoder utilizing GRU layers reconstructing a 24 hour data sequence, a transformer predicting
the next hour given the 24 previous hours, and the DeepAnT, also predicting the next hour given the 24 previous hours. After training, the models were evaluated together on data sequences containing possible but not definitive, anomalies. The results show clear differences between the predictive models and the auto-encoder. Where the predictive models tend to simply follow the trend of the previous hour, the auto-encoder is much better at generalizing and therefore, are less subject to follow sudden anomalies. However, none of the models were able to identify anomalies happening over the course of multiple weeks or months.

### Repository 

The project consist of four iPython notebooks, that contain the three different models and a notebook for evaluating the models and compare their performance with respect to each other.

The data used troughout the project is not uploaded to Github since this is not publicly available. 
* Model folder: Contains the trained models along with threshold values for anomaly detection in .pt files 
* Code folder: Contains the four notebooks(.ipynb files)


