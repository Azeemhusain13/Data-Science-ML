Cyclone Preheater Anomaly Detection
Project Overview
This project analyzes operational data from a cyclone preheater, which is part of an industrial process. The primary objective is to identify periods of abnormal operations using machine learning techniques, particularly Isolation Forest for anomaly detection. The dataset consists of 370k records collected over a duration of 3 years, with data recorded every 5 minutes.

Dataset Information
The dataset contains the following key variables:

Cyclone_Inlet_Gas_Temp: Temperature of hot gas entering the cyclone.
Cyclone_Gas_Outlet_Temp: Temperature of hot gas leaving the cyclone.
Cyclone_Outlet_Gas_draft: Draft (pressure) of gas at the outlet of the cyclone.
Cyclone_cone_draft: Draft (pressure) of gas at the cone section of the cyclone.
Cyclone_Inlet_Draft: Draft (pressure) of gas at the inlet of the cyclone.
Cyclone_Material_Temp: Temperature of the material at the outlet of the cyclone.
Objective
The objective of this project is to:

Detect anomalous operations within the cyclone preheater using historical data.
Identify periods of sharp deviations in temperature and pressure that may indicate system malfunctions or inefficiencies.
Methodology
1. Data Preprocessing:
Missing Values: Missing data was imputed using mean imputation to ensure completeness.
Conversion: Ensured that temperature and pressure columns were converted to numeric values for analysis.
Datetime Conversion: The time column was converted into datetime format for time series analysis.
2. Anomaly Detection:
Algorithm: Applied Isolation Forest to detect anomalies based on the six key variables.
Contamination: Set contamination to 1%, meaning 1% of data points were flagged as anomalies.
Features Used: The model considered all six features, including temperatures and drafts, for anomaly detection.
3. Insights:
The algorithm detected anomalies during periods of sharp fluctuations in gas temperature and pressure.
These abnormalities could indicate potential issues such as gas flow disruptions or equipment malfunctions.
Results
1% of the data was flagged as anomalies, indicating potential periods of abnormal operation.
Detected anomalies were visualized, with Cyclone Inlet Gas Temperature plotted over time, highlighting abnormal points in red.
Requirements
To run this project, you need the following libraries:

pandas
numpy
scikit-learn
matplotlib

How to Run the Code
Clone this repository to your local machine.
presentation/: PowerPoint presentation summarizing data preparation, analysis strategy, and insights.
Conclusion
This project provides insights into the abnormal periods during cyclone preheater operations and demonstrates the use of Isolation Forest for detecting anomalies in industrial processes. These findings can be used for preventive maintenance and process optimization.
