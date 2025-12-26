# FitPulse Health Anomaly Detection from Fitness Devices
## Milestone 2: Feature Extraction and Modeling


## Objective
The objective of Milestone 2 is to extract meaningful statistical and time-series features
from fitness device data, model temporal trends, and identify behavioral patterns using
unsupervised learning techniques. This milestone forms the foundation for anomaly detection
in subsequent milestones.


## Dataset Description
The project uses fitness tracker data collected from wearable devices. The datasets include:

- Heart rate time-series data
- Daily step count data
- Sleep duration data

The data is sourced from a public Fitbit Fitness Tracker Dataset and contains timestamped
measurements suitable for time-series analysis.


## Feature Extraction
Statistical features are extracted from the heart rate time-series data, including:
- Mean
- Standard Deviation
- Minimum and Maximum values
- Skewness
- Kurtosis

These features help summarize overall physiological behavior over time.


## Trend Modeling
Facebook Prophet is used to model temporal trends and seasonality in heart rate data.
The model forecasts expected values and residuals are computed to identify deviations
from normal patterns.

Visualizations with confidence intervals are generated to better understand behavioral trends.


## Clustering Behavioral Patterns
Unsupervised learning techniques are applied to group behavioral patterns:
- KMeans clustering is used to classify behavior into normal and atypical groups
- PCA is used for dimensionality reduction and visualization of clusters

These clusters provide insight into different user behavior patterns.

## Tools and Technologies Used
- Python
- Google Colaboratory
- Pandas & NumPy
- Matplotlib
- Scikit-learn
- Facebook Prophet
- TSFresh (optional)


## Key Observations
- Statistical features effectively summarize fitness behavior
- Prophet captures seasonal and long-term trends
- Clustering separates behavioral patterns into meaningful groups
- PCA enables clear visualization of clustered behavior


