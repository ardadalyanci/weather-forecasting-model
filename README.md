# Time-Series Weather Forecasting Model 🌦️

This project demonstrates a complete end-to-end machine learning workflow for time series forecasting. It uses a Python script to fetch multi-year historical weather data from the official NOAA (National Oceanic and Atmospheric Administration) API. The data is then cleaned, processed, and used to train a machine learning model to predict the maximum daily temperature.

## Final Result
The final `RandomForestRegressor` model achieves a Mean Absolute Error (MAE) of approximately **3.4°F** on the test set, demonstrating its ability to accurately forecast daily maximum temperatures.

### Prediction Visualization
The plot below compares the model's predicted temperatures (orange) against the actual temperatures (blue) on the unseen test data.
![Actual vs. Predicted Plot]
<img width="2471" height="1127" alt="image" src="https://github.com/user-attachments/assets/7e219e5e-eef5-4f75-8ca2-5dd579ef29a0" />


## Key Features
- Fetches multi-year historical data from the NOAA Climate Data Online API.
- Cleans and prepares raw API data into a usable time series format using Pandas.
- Performs feature engineering by extracting `month`, `day_of_year`, `day_of_week`, and `lag` features.
- Trains and evaluates multiple models, including `RandomForestRegressor`.
- Evaluates model performance using Mean Absolute Error (MAE).
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
    git clone [https://github.com/ardadalyanci/weather-forecasting-model.git](https://github.com/ardadalyanci/weather-forecasting-model.git)
    cd weather-forecasting-model
    ```

2.  **Create a `requirements.txt` file:**
    Create a file named `requirements.txt` and paste the following lines into it. This is the standard way to manage project dependencies.
    ```text
    pandas
    requests
    scikit-learn
    matplotlib
    ```

3.  **Install dependencies:**
    Run the following command in your terminal to install all the necessary libraries from your `requirements.txt` file.
    ```bash
    pip install -r requirements.txt
    ```

4.  **Get a NOAA API Token:**
    - Visit the [NOAA Token Request page](https://www.ncdc.noaa.gov/cdo-web/token) and get a free API token sent to your email.

5.  **Update the Script:**
    - Open the Python script/notebook and replace `'YOUR_TOKEN_HERE'` with the token you received.

6.  **Run the script:**
    - Execute the Python script or run the cells in the notebook to fetch the data, train the model, and see the results.
