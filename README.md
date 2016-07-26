# RandomForests

This project applies a random forest to the problem of predicting flight delays based on year, month, day of month, day of week, departure time, airport of origin, airport of destination, airline, and flight distance.

See blog post at [lucdemortier.github.io](http://lucdemortier.github.io/articles/16/RandomForestsWiMLDS) for a description of the results.

This repository contains the Jupyter notebook used for the analysis, FlightDelayPrediction.ipynb, with code to perform the following calculations:

1. Read airline data into Pandas dataframe, clean up, and compute basic statistics.

1. Plot normalized feature distributions for delay and no-delay subsamples.

1. Compute intrinsic discrepancies.

1. Convert categorical variables into binary ones.

1. Recompute intrinsic discrepancies.

1. Split data set into training and testing parts, with option to adjust the prevalence in either part.

1. Do a quick preliminary fit of a random forest classifier to the training data set, to make sure things are working as expected.

1. Do grid search to optimize hyper-parameter settings of random forest.

1. Compute confusion matrix of optimal random forest and plot precision, recall, and queue rate versus threshold curves, as well as the ROC, a bar chart of feature importances, and histograms of the classifier output.

1. Investigate the variability of the precision, recall, and queue rate versus threshold curves.
