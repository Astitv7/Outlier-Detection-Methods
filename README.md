# Outlier-Detection-Methods

**Anomalies**, or **Outliers**, can be a serious issue when training machine learning algorithms or applying statistical techniques. They are often the result of errors in measurements or exceptional system conditions and therefore do not describe the common functioning of the underlying system. Indeed, the best practice is to implement an outlier removal phase before proceeding with further analysis.

But hold on there! In some cases, outliers can give us information about localized anomalies in the whole system; so the detection of outliers is a valuable process because of the additional information they can provide about your dataset.

## Outlier Detection Techinques
1. **Percentile**
- In this method we try to remove to outliers using our domain knowledge.

2. **Z-Score**
- This technique assumes a Gaussian distribution of the data. The outliers are the data points that are in the tails of the distribution and therefore far from the mean. How far depends on a set threshold zthr for the normalized data point
- An outlier is then a normalized data point which has an absolute value greater than zthr.

3. **IQR**
- The outliers are calculated by means of the IQR (InterQuartile Range). For example, the first and the third quartile (Q1, Q3) are calculated. An outlier is then a data point xi that lies outside the interquartile range.
- Using the interquartile multiplier value k=1.5, the range limits are the typical upper and lower whiskers of a box plot.
