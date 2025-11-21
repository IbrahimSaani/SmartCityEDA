# Smart City Sensor Data – Exploratory Data Analysis (EDA)

 1. Project Overview
This project analyzes IoT sensor data collected at 5-second intervals over one week.  
The dataset is aimed at improving smart city monitoring and understanding environmental trends.

 Sensor Measurements:
- Temperature
- Humidity
- Light
- pH
- Electrical Conductivity (EC)

  Data Source: 
Grant No. BR24992852 – “ Intelligent models and methods of Smart City digital ecosystem for sustainable development and the citizens’ quality of life improvement ”

---

 2. Project Structure

  text
SmartCityEDA/
├─ data/                 # CSV files (one per day)
├─ plots/                # Automatically saved charts
├─ smart_city_eda.ipynb  # Jupyter notebook (EDA)
└─ README.md             # report

 3. Steps in EDA (Notebook Summary)

Load and combine all CSV files

View .info() and .describe()

Handle time column → Extract date and hour

Plot temperature, humidity, and light over time

Identify day–night light cycle using hourly averages

Compute correlations between sensors

Calculate mean, min, max, and variance for each sensor

Save plots automatically for the README

4. Key Observations

Light values increase between 6 AM and 6 PM, showing a strong day–night cycle.

Humidity decreases when temperature rises, showing an inverse relationship.

Peak temperature occurs around 2 PM, matching typical outdoor weather patterns.

pH and electrical conductivity remain stable, suggesting controlled environment.

5. Sample Plots

Below are examples of the saved plots from the notebook:

Daily Trend (Temperature, Humidity, Light)
![alt text](plots/daily_temp_hum_light.png)

Hourly Light Pattern
![alt text](plots/hourly_light_pattern.png)

Correlation Heatmap
![alt text](plots/correlation_temp_hum_light.png)

6. Conclusions

IoT sensors are reliable for real-time monitoring.

Environmental changes follow natural daily cycles.

Data can be used for prediction models, climate monitoring, and smart city planning.

7. Technologies Used

| Tool                 | Purpose       |
| -------------------- | ------------- |
| Python 3.10          | Programming   |
| pandas               | Data handling |
| matplotlib & seaborn | Visualization |
| VS Code              | Development   |
| Jupyter Notebooks    | EDA           |

8. Future Work

Add machine learning for anomaly detection

Build a dashboard using Streamlit or Flask

Predict humidity or temperature trends using time-series models

9. How to Run

 Create virtual environment
python -m venv .venv
.venv\\Scripts\\Activate.ps1

 Install dependencies
pip install pandas matplotlib seaborn

 Open the notebook in VS Code
smart_city_eda.ipynb


