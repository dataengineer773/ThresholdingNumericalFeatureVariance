We have a set of numerical features and want to filter out those with low variance, Select a subset of features with variances above a given threshold, Variance thresholding (VT) is an example of feature selection by filtering, and one of the most basic
approaches to feature selection. It is motivated by the idea that features with low variance are likely less
interesting (and useful) than features with high variance. VT first calculates the variance of each feature, where x is the feature vector, xi
is an individual feature value, and μ is that feature’s mean value. Next, it
drops all features whose variance does not meet that threshold.
There are two things to keep in mind when employing VT. First, the variance is not centered; that is, it
is in the squared unit of the feature itself. Therefore, the VT will not work when feature sets contain
different units (e.g., one feature is in years while a different feature is in dollars). Second, the variance
threshold is selected manually, so we have to use our own judgment for a good value to select (or use a
model selection technique described in [Link to Come]). We can see the variance for each feature using
variances_ , Finally, if the features have been standardized (to mean zero and unit variance), then for obvious
reasons variance thresholding will not work correctly, 
