---
layout: post
title: Fourth Post- Project 2- Creating data summaries, predictive models, and automated Markdown reports from the Bike Sharing Dataset
---
In this project, Jiashu Zhao and I were given the task of creating data summaries, predictive models, and automated Markdown reports from the 
[bike sharing data set](https://archive.ics.uci.edu/ml/datasets/Bike+Sharing+Dataset) using functions from the `readr`,`ggplot2`, `dplyr`, `knitr`,`caret`,`tidyr`,`lubridate`,
`leaps`,`regclass`, and `MASS` packages. The day.csv file was used throughout.

My roles in this collaboration included setting up the project repo, reading in the data and splitting it into the training and testing subsets, producing some of the summary
statistics and plots, creating one linear regression and Random Forest model, and writing part of the code used to compare the four models.

Overall, Jiashu and I collaborated very effectively (despite the 12 hrs difference in our local timezones!) and either one of us was able to figure out the different obstacles we 
faced during the course of the project. The most difficult part for me was figuring out how to compare the four models. We elected to use the `count` variable as the response, but 
could not use missclassification rate as a basis for comparison because the response variable is not binary. After numerous Google searches, I proposed using the RMSE as the basis,
and it seems to work quite well. Although we were able to use RMSE to select between models, the RMSE values were generally pretty high, which makes me think our model candidates 
choices leaves a lot to be desired.

Like the first project, this project further increased my familiarity with R. One big takeaway from this project was that there's no one size fits all when it comes to the best 
predictive model. During the course of the project I perused a number of journal articles that used model comparison for better response predictions ([this article](https://pubmed.ncbi.nlm.nih.gov/24012917/) 
was a particular highlight) and I am already thinking of how I can utilize predictive modeling with response surface methodology at work.

[Github repo](https://github.com/yemoray/ST-558-Project_2)  
[Github page](https://yemoray.github.io/ST-558-Project_2/)
