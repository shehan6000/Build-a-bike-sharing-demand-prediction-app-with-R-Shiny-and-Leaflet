# Bike-Sharing Demand Prediction with Weather Forecast Data

This project uses weather forecast data to predict bike-sharing demand in various cities. The main script is written in R and utilizes the `tidyverse` and `httr` packages.

## Overview

The script performs the following tasks:

1. **Fetches weather forecast data**: The `get_weather_forecaset_by_cities` function fetches 5-day weather forecast data for a list of cities using the OpenWeatherMap API.

2. **Loads a saved regression model**: The `load_saved_model` function loads a saved regression model from a CSV file. This model is used to predict bike-sharing demand based on weather conditions.

3. **Predicts bike-sharing demand**: The `predict_bike_demand` function uses the loaded regression model to predict bike-sharing demand based on temperature, humidity, wind speed, visibility, season, and hour of the day.

4. **Defines bike-sharing demand level**: The `calculate_bike_prediction_level` function categorizes the predicted bike-sharing demand into three levels: small, medium, and large. This categorization is used for visualization purposes.

5. **Generates a data frame containing weather forecasting and bike prediction data**: The `generate_city_weather_bike_data` function generates a data frame that contains weather forecasting and bike prediction data for each city.

## Usage

To use this script, you need to have R installed along with the `tidyverse` and `httr` packages. You also need to replace the OpenWeatherMap API key in the `get_weather_forecaset_by_cities` function with your own.

Please note that this script assumes that you have a CSV file named "selected_cities.csv" that contains the list of cities for which you want to fetch weather forecast data and predict bike-sharing demand. It also assumes that you have a saved regression model in a CSV file named "model.csv".

## Disclaimer

This script is provided as-is, and it is recommended to review and adjust it according to your needs and context. The accuracy of the predictions depends on the quality and relevance of the weather forecast data and the regression model used.
