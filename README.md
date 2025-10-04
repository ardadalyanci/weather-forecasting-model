# Time-Series Weather Forecasting Model

This project is an end-to-end machine learning workflow for time series forecasting. It uses a Python script to fetch multi-year historical weather data from the official NOAA (National Oceanic and Atmospheric Administration) API. The data is then cleaned, processed, and used to train a machine learning model to predict the maximum daily temperature.

## Features
- Fetches multi-year historical data from the NOAA Climate Data Online API.
- Cleans and prepares raw API data into a usable time series format using Pandas.
- Performs feature engineering by extracting `month`, `day_of_year`, `day_of_week`, and `lag` features.
- Trains a `RandomForestRegressor` model to forecast future temperatures.
- Evaluates the model's performance using Mean Absolute Error (MAE).
- Visualizes the model's predictions against actual values using Matplotlib.

## Technologies Used
- Python
- Pandas
- Scikit-learn
- Matplotlib
- Requests
- NOAA Climate Data Online API

## Setup and Usage

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/your-username/weather-forecasting-model.git](https://github.com/your-username/weather-forecasting-model.git)
    cd weather-forecasting-model
    ```

2.  **Install dependencies:**
    ```bash
    pip install pandas requests scikit-learn matplotlib
    ```

3.  **Get a NOAA API Token:**
    - Visit the [NOAA Token Request page](https://www.ncdc.noaa.gov/cdo-web/token) and get a free API token sent to your email.

4.  **Update the Script:**
    - Open the Python script/notebook and replace `'YOUR_TOKEN_HERE'` with the token you received.

5.  **Run the script:**
    - Execute the Python script or run the cells in the notebook to fetch the data, train the model, and see the results.
