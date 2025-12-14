# FitPulse Health Anomaly Detection from Fitness Devices
## Milestone 1: Data Collection and Preprocessing

### Objective
To collect and preprocess fitness data from wearable devices, normalize timestamps, handle missing values, and align data to a 1-minute interval for anomaly detection.

### Dataset Source
Fitbit Fitness Tracker Dataset (CSV format)

### Steps Performed
1. Loaded CSV datasets using Pandas
2. Converted timestamps to UTC format
3. Handled missing values using forward fill and zero imputation
4. Resampled heart rate data to a 1-minute interval
5. Aligned activity and sleep data to the same interval
6. Merged datasets using user ID and timestamp
7. Generated a clean consolidated dataset

### Tools Used
- Python
- Pandas
- NumPy
- Google Colab

### Output
- Clean dataset: `Clean.csv`

### Screenshots
Screenshots are available in the Screenshot folder.
