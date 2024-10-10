FHR and UC Analysis
This project analyzes a dataset containing Fetal Heart Rate (FHR) and Uterine Contractions (UC) data. The key objectives include plotting graphs, analyzing FHR over time, and detecting peaks in UC to provide insights.

Project Structure
main.ipynb: Python script that performs the data loading, plotting, FHR analysis, and UC peak detection.

Simulator_readings.csv: The dataset containing the following columns:

Time(ms): Time in milliseconds.
Fhr1(BPM): Fetal heart rate 1 in beats per minute.
Fhr2(BPM): Fetal heart rate 2 (can be ignored if all values are zero).
Uc(TOCO): Uterine contractions data.
README.md: This file, which provides details about the project.

Outputs
Time vs FHR1 Graph: Displays the Fetal Heart Rate over time.
Time vs UC Graph: Displays Uterine Contractions over time.
FHR Analysis: Calculates the average FHR over epochs of 3.75 seconds and computes pulse intervals.
UC Peak Detection: Detects peaks in UC values and calculates the number of peaks wider than 30 seconds, as well as the average duration of these peaks.

File Descriptions
Simulator_readings.csv: Contains the FHR and UC data used for the analysis.
main.ipynb: The Python script that performs all analyses, including:
Plotting Time vs FHR1 and Time vs UC graphs.
Performing FHR analysis over 3.75-second epochs.
Detecting UC peaks and calculating the width and duration of significant peaks.

Requirements:
pandas
matplotlib
scipy
