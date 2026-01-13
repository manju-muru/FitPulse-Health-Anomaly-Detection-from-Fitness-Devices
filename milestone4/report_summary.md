Objective:

The objective of this milestone is to develop and deploy an interactive health anomaly dashboard that visualizes user fitness data and detects unusual patterns. The dashboard enables users to upload their data, automatically processes it, highlights abnormal behavior, and provides downloadable reports for future analysis.

Dashboard Workflow:

Data Upload
Users upload a CSV or JSON file containing fitness metrics such as steps, sleep duration, and heart rate.
The dashboard automatically reads and standardizes column names.
Data Preprocessing
Converts related fields (e.g., sleep minutes to hours if required).
Cleans inconsistent column naming (avg_heart_rate → heart_rate, step_count → steps, etc.)
Adds missing date values if required using daily indexing.

Anomaly Detection:

Heart rate anomaly detection identifies days with heart rate values outside normal thresholds.
Sleep anomaly detection detects unusually short or long sleep durations.
Step count anomaly detection flags abnormally low or high activity levels.

Visualization:

Displays a preview of the raw uploaded dataset.
Plots line charts for heart rate, sleep hours, and step counts with anomaly points highlighted.
Provides summary metrics showing the total number of anomalies detected in each category.

Report Export:

Generates a structured anomaly output.
Allows users to download the cleaned and labeled dataset as a CSV file.

Tools and Libraries Used:

Python
Pandas for data cleaning and preprocessing
Streamlit for dashboard user interface
Plotly Express for interactive visualizations
Google Colab for development and testing environment

Key Insights from the Dashboard:

Heart rate anomalies can indicate days of high physical stress, low heart activity, or sensor errors.
Sleep pattern anomalies reveal irregular routines that may be linked to health, stress levels, or lifestyle changes.
Step anomalies track unusually active or inactive days, helping assess overall activity levels.
The system adapts to multiple datasets through flexible column recognition and automatic formatting.
Downloadable anomaly summaries make it easy for users to document findings or integrate results into later milestones.

Screenshot References:

Screenshot showing full dashboard with upload, metrics, and graphs.
Screenshot highlighting the anomaly counts displayed via metric cards.
Screenshot showing the download button and exported CSV format.