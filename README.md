# aai-iot-cleaning-and-eda
Household Electric Power Consumption Analysis
Overview
This Python application performs exploratory data analysis (EDA) and data cleaning on a dataset containing household electric power consumption data. The goal of this project is to analyze the data, clean it, and provide insights into the household's electricity usage. The project uses Python libraries like pandas, matplotlib, seaborn, and numpy for various analysis and visualization tasks.
Features
•	Data Preprocessing: Handles missing values, outlier detection, and data type conversions.
•	Exploratory Data Analysis (EDA): Visualizes the distribution and relationships of key features like voltage, global active power, and time-based trends.
•	Data Cleaning: Filters out outliers, handles missing values, and converts data types as necessary.
•	Data Visualization: Creates various plots (histograms, scatter plots, time series plots) to help understand patterns in the data.
Libraries Used
•	pandas: For data manipulation and cleaning.
•	numpy: For numerical computations.
•	matplotlib: For data visualization (plots).
•	seaborn: For advanced statistical visualizations.
•	datetime: For handling date and time-related operations.
•	scipy: For statistical analysis (optional).
Dataset
The dataset used in this project is from the UCI Machine Learning Repository, specifically the Household Power Consumption dataset. It contains measurements of electric power consumption in one household over a period of time (from 2006 to 2010).
Dataset can be downloaded from:
UCI Household Power Consumption Dataset
Dataset Columns
•	Date: The date when the measurement was taken (formatted as "day/month/year").
•	Time: The time when the measurement was taken (formatted as "hh:mm:ss").
•	Global_active_power: The global active power in kilowatts.
•	Global_reactive_power: The global reactive power in kilowatts.
•	Voltage: The voltage in volts.
•	Global_intensity: The intensity of the global power in amperes.
•	Sub_metering_1: Energy sub-metering in watt-hours (for kitchen).
•	Sub_metering_2: Energy sub-metering in watt-hours (for laundry room).
•	Sub_metering_3: Energy sub-metering in watt-hours (for air conditioning).
Installation
To run this application locally, you need Python installed along with the required libraries. You can set up a Python environment and install dependencies using the following steps.
1.	Clone this repository:
2.	git clone https://github.com/yourusername/household-electric-power-consumption.git
3.	cd household-electric-power-consumption
4.	Install the required libraries:
5.	pip install -r requirements.txt
6.	If you don't have requirements.txt, manually install the dependencies:
7.	pip install pandas numpy matplotlib seaborn
How to Use
1.	Load the Dataset: Load the dataset using pandas for analysis:
2.	import pandas as pd
3.	data = pd.read_csv('household_power_consumption.txt', sep=';', low_memory=False)
4.	Data Cleaning:
o	Convert the Date and Time columns into a proper datetime format.
o	Handle missing values and filter out invalid data.
o	Clean numerical columns for potential issues such as negative values or outliers.
5.	Exploratory Data Analysis (EDA):
o	Perform basic statistical summary of the data using .describe().
o	Visualize power consumption trends over time using time series plots.
o	Create histograms and scatter plots to examine the distribution and correlations of key features.
6.	Visualization Example: Create a time series plot for Global_active_power:
License
This project is licensed under the MIT License - see the LICENSE file for details.
