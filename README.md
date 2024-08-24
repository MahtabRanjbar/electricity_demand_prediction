# Ontario Electricity Demand and Price Forecasting Project

## Project Overview
This project explores forecasting the Hourly Ontario Energy Price (HOEP) and Ontario electricity demand using historical data that includes weather variables like temperature, wind speed, and humidity. The goal is to provide accurate short-term predictions for energy market participants. This project employs time series modeling, specifically using a Vector Autoregression (VAR) model.


## Data
The dataset includes hourly records spanning January 1, 2016, to January 2, 2016. Below are the primary features:

- Date: Date of the observation.
- Weekday: Day of the week (e.g., Friday).
- Hour: Hour of the day (0-23).
- HOEP: Hourly Ontario Energy Price (in CAD).
- Ontario_Demand: Hourly electricity demand in Ontario (in MW).
- Temperature (°C): Measured temperature.
- Windchill_Index (°C): Wind chill effect on temperature.
- Wind_Speed (km/h): Speed of the wind.
- Humidex: Combined effect of temperature and humidity.
- Relative_Humidity (%): Relative humidity percentage.
- Dew_Point (°C): Dew point temperature.
- Pressure_Station (kPa): Atmospheric pressure.

## Getting Started
To get started with this project, clone the repository and install the required dependencies.
1. Clone this repository:
    ```bash
    git clone https://github.com/MahtabRanjbar/emergency_call_analysis.git
    ```
2. Install the required packages:
    ```bash
    pip install -r requirements.txt
    ```

##Exploratory Data Analysis
Initial data exploration and visualization include:

- Analyzing the relationship between HOEP, demand, and weather factors.
- Visualizing hourly and daily trends in energy demand.
- Investigating correlations between price spikes and temperature drops.
Key findings:

- Strong inverse relationships between HOEP and temperature during winter.
- Higher demand observed during colder hours, with price spikes coinciding.

## Modeling Approach
### Model Selection
This project employs a Vector Autoregression (VAR) model due to its ability to handle multivariate time series. It captures interdependencies between HOEP, electricity demand, and weather conditions.

### Model Training and Validation
- The data was split into training and test sets.
- Walk-forward validation was used to ensure robust predictions.
- Forecast performance was measured using metrics like RMSE and MAE.

### Challenges
- Handling missing data and outliers.
- Accounting for seasonality and trend components in the data.

## License
This project is licensed under the MIT License. See the LICENSE file for more details.

