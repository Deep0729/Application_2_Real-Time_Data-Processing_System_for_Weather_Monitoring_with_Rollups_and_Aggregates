# Real-Time_Data-Processing_System_for_Weather_Monitoring_with_Rollups_and_Aggregates


## Hosted Link: https://deep0729.github.io/Application_2_Real-Time_Data-Processing_System_for_Weather_Monitoring_with_Rollups_and_Aggregates/


 ![Screenshot 2024-10-18 110319](https://github.com/user-attachments/assets/191a6e72-9b30-4063-80b9-9d319615330d)

 ![Screenshot 2024-10-18 112254](https://github.com/user-attachments/assets/243c98a3-6417-4b6d-b311-ae1847165605)

 ![Screenshot 2024-10-18 110407](https://github.com/user-attachments/assets/87098369-c9e7-4542-8f70-1ba1aada4a15)


## Overview

This project is designed to retrieve weather data from the OpenWeatherMap API at configurable intervals, convert temperature values based on user preference, and provide daily weather summaries including additional parameters like humidity and wind speed. The system is built to be robust, easy to set up, and extendable.

## Features

- **System Setup:** Initializes and connects to the OpenWeatherMap API using a valid API key.
- **Data Retrieval:** Simulates API calls at configurable intervals to retrieve and parse weather data for specified locations.
- **Temperature Conversion:** Converts temperature values from Kelvin to Celsius or Fahrenheit based on user preference.
- **Daily Weather Summary:** Simulates weather updates over several days and calculates average, maximum, minimum temperatures, and dominant weather conditions.
- **Additional Parameters:** Supports retrieval and analysis of additional weather parameters such as humidity and wind speed.
- **5 days Weather Forecast**
- **main:** Main weather condition (e.g., Rain, Snow, Clear)
- **temp:** Current temperature in Centigrade
- **feels_like:** Perceived temperature in Centigrade
- **dt:** Time of the data update (Unix timestamp)

## Design Choices

- **Modularity:** The system is divided into distinct modules for initialization, data retrieval, temperature conversion, and summary generation, making it easy to maintain and extend.
- **Configurability:** API call intervals and temperature units are configurable to allow flexibility.
- **Extensibility:** Designed to easily incorporate additional weather parameters from the OpenWeatherMap API.

## Rollups and Aggregates:

**1. Daily Weather Summary:**
 -  Roll up the weather data for each day.
**Calculate daily aggregates for:**
    - Average temperature
    - Maximum temperature
    - Minimum temperature
    - Dominant weather condition (give reason on this)
**Store the daily summaries in a database or persistent storage for further analysis.**

**2. Alerting Thresholds:**
  - Define user-configurable thresholds for temperature or specific weather
    conditions (e.g., alert if temperature exceeds 35 degrees Celsius for two
    consecutive updates).
  - Continuously track the latest weather data and compare it with the thresholds.
  - If a threshold is breached, trigger an alert for the current weather conditions.
    Alerts could be displayed on the console or sent through an email notification
    system (implementation details left open-ended).

**3. Implement visualizations:**
  - To display daily weather summaries, historical trends, and triggered alerts.

## Requirements
- Screen 1070*680 minimum
- Nodejs (optional in case system do not have live server utility)

## Getting Started

### Prerequisites

- Node.js and npm installed

### Installation

1. **Clone the Repository**
   ```bash
   git clone "https://github.com/Deep0729/Application_2_Real-Time_Data-Processing_System_for_Weather_Monitoring_with_Rollups_and_Aggregates.git"
   ```

2. **Install Backend Dependencies (Optional)**

   ```bash
   npm install
   
   ```
   
3. **run live server

   ```bash
   npm install http-server -g
   ```
   
   ```
   http-server -p 8080**
   ```
   
   ** After run the command in the terminal it shows available links in the terminal. For example:
    ```
    http://192.168.29.96:8080
    ```
    or
   ```
   http://127.0.0.1:8080
   ```
   This is for my terminal.
   You can click the link using (ctrl+click). So you can redirect to another tab and you can get real time weather update according to your choice.

## Running Tests

You can add and run tests to ensure everything is working correctly.
```
created bt: Deep Dutta
```

## Thank You
