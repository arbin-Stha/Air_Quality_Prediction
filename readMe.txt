# Air Quality Predictor

## Overview
The Air Quality Predictor is a web application designed to estimate PM2.5 levels (a key air pollutant) based on user-provided environmental factors such as temperature, humidity, wind speed, and PM10 levels. Additionally, the app displays the relative impact of these factors in a pie chart and categorizes the air quality based on the predicted PM2.5 level.

## Features
- User-friendly web interface to input environmental parameters.
- Predict PM2.5 concentration using a trained machine learning model.
- Display the level of concern based on PM2.5 predictions.
- Visualize the contribution of various factors using a pie chart.

## Technologies Used
- **Backend**: Django (Python-based web framework)
- **Frontend**: HTML, CSS, Bootstrap
- **Machine Learning**: Scikit-learn (Linear Regression model)
- **Visualization**: Matplotlib for generating pie charts
- **Data Handling**: Pandas for data manipulation

## Installation
### Prerequisites
Ensure you have the following installed:
- Python 3.8+
- Django 4.0+
- Scikit-learn
- Matplotlib
- Pandas

### Steps
1)install
  pip install scikit-learn
  pip install streamlit pandas scikit-learn matplotlib
  pip install matplotlib


 



2. Start the development server:
   myenv\Scripts\Activate
   python manage.py runserver
   

3. Open the application in your browser at `http://127.0.0.1:8000/`.

## Usage
1. Navigate to the homepage of the application.
2. Fill in the required environmental parameters:
   - Temperature (°C)
   - Dew Point (°C)
   - Humidity (%)
   - Wind Speed (Kph)
   - Pressure (Hg)
   - Precipitation (mm)
   - PM10 (µg/m³)
3. Click the **Predict** button.
4. View the predicted PM2.5 level, level of concern, and the pie chart illustrating factor contributions.

## Levels of Concern
The application categorizes the air quality based on PM2.5 levels as follows:
- **Good**: PM2.5 <= 50
- **Moderate**: 51 <= PM2.5 <= 100
- **Unhealthy for Sensitive Groups**: 101 <= PM2.5 <= 150
- **Unhealthy**: 151 <= PM2.5 <= 200
- **Very Unhealthy**: 201 <= PM2.5 <= 300
- **Hazardous**: PM2.5 > 300
## Example Dataset
The application uses a preprocessed dataset (`cleaned_weather_data1.csv`) containing historical air quality and weather data for training and predictions.

## Future Enhancements
- Include additional environmental factors for more accurate predictions.
- Support for real-time data collection via APIs.
- Implement more advanced machine learning models for prediction.

## License
This project is licensed under the MIT License. See the LICENSE file for details.

## Contributing
Contributions are welcome! Feel free to open issues or submit pull requests to improve the application.

---
Thank you for using the Air Quality Predictor! If you encounter any issues or have feedback, please let us know.

