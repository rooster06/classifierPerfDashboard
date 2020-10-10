# Binary Classifier Performance Dashboard

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/rooster06/classifierPerfDashboard/main?urlpath=voila%2Frender%2FClassifierPerfDashboard.ipynb)

Dashboard to view binary classifier performance metrics and tune threshold for binary prediction

[Binary Classifiers](https://en.wikipedia.org/wiki/Binary_classification) are widely used for various tasks in ML & Data Science. Regardless of the choice of ML algorithms (Logistic, Tree based or Neural Nets), a binary classifiers performance is often optimized or measured based on a select few metrics like AUC-ROC, F-score, etc. 

This App is an attempt to allow ML/DS practitioners more time to understand their results by the way of
- Automating the process of creating some of the popular metrics
- Creating an informative visual dashboard to aid optimal threshold selection

**Metrics of interest in this App**
- AUC-ROC curve & AUC
- N-tile (x-axis) V Target rate (Y-axis) charts - useful viz for how well your model slopes target
- Best possible F-scores and the corresponding threshold values and confusion matrices
- For a threshold of users choosing F-scores and the confusion matrix


    
<h3><center>Directions For Use:</center></h3>   

    
1. Upload a csv with two columns- target variable and model predictions
2. You will see an AUC-ROC curve & the AUC measure
3. Select the number of buckets(n-tile) using the slider for the N-tile V Target rate chart
4. Row 2 conatins the best possible F-scores and corresponding thresholds, confusion matrices. 
5. Adjust the slider to a threshold of your choosing to create the corresponding metrics - precision, recall and confusion matrix.

<div class="Note:">
  .Note: .bg-red
</div>Column names must be target and preds, the target variable must be dichotomous only taking the values 0 and 1
