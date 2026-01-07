Milestone 3 — Anomaly Detection Report

 Objective:
The goal of Milestone 3 was to detect unusual patterns in Fitbit user data—
particularly heart rate and sleep duration—by applying data-driven anomaly
detection techniques. Detecting anomalies helps identify potential health issues,
stress periods, unusually inactive days, or device tracking errors.


Steps Followed:
 1. Data Cleaning & Transformation
 Extracted time-series components from Fitbit logs
 Aggregated records to per-hour or per-day where required
 Filled or removed missing values to ensure model consistency

 2. Residual Analysis
Computed expected signal using rolling averages
Calculated residuals = actual − expected
Large deviations flagged for deeper processing

 3. Thresholding
Applied dynamic Z-score/σ rule (e.g., ±2–3 standard deviations
 Quickly identifies extreme outliers without ML assumptions

 4. Cluster-Based Detection
 Implemented DBSCAN to separate normal vs abnormal points
 Captured behavior anomalies that are not purely numeric outliers
 Useful for irregular patterns not detected by thresholds

 5. Visualization
 Generated clear anomaly plots:
 Heart Rate anomaly timeline
 Sleep duration anomaly scatter
 Anomaly points highlighted visually for interpretation


Tools Used
Python
pandas – data preprocessing
numpy – statistical operations
matplotlib – plotting anomaly charts
Scikitlearn – DBSCAN clustering
datetime– time feature extraction


 Key Insights & Observations
Heart rate data revealed spikes at irregular times likely linked to high activity bursts or stress.
Sleep logs identified several days with:
Very low sleep duration (<4–5 hrs)
unusually long sleep (>10 hrs)
Cluster-based detection captured subtle patterns missed by thresholding alone.
Combining residual analysis, statistical thresholds, and clustering improves
 reliability vs using any single method.

 Conclusion
Milestone 3 demonstrates that a hybrid anomaly detection pipeline can successfully
flag unusual biometric behavior. These insights form the foundation for future
features such as:
- Alert systems to notify users of abnormal patterns
- Personalized health recommendations
- Predictive modeling in Milestone 4