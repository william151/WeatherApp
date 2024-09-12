#WeatherApp - SwiftUI

WeatherApp is a weather forecasting application built with SwiftUI, allowing users to get real-time weather data based on their location or by searching for a specific city. This project is designed with a clean architecture and demonstrates the use of modern SwiftUI features along with API integration.

# Features

- Real-time Location Weather: Automatically fetches weather data based on the user's current location.
- Weather Details: Displays data like temperature, humidity, wind speed, and forecast.
- Elegant UI: Built with SwiftUI to provide a smooth and responsive user experience.
- Error Handling: Gracefully handles network and API errors.

# Project Structure

The project is structured to separate concerns and keep the code modular and maintainable. Below is a description of the key files and folders in the project:

# Files and Directories
- WeatherApp.swift
The main entry point of the app. It initializes the app's environment and launches the main view.
- ContentView.swift
This file contains the primary user interface of the app, which displays the weather details based on either the user's location or searched city.
- WeatherManager.swift
This is the core service file responsible for fetching weather data from the API. It uses URLSession to make network calls and decodes the JSON responses into Swift models.
- WeatherData.swift
A model file that defines the data structures for parsing the JSON response from the weather API. This ensures that the app can handle and display the weather data in the UI.
- LocationManager.swift
Handles location-related functionality, including requesting permission to access the user's location and retrieving latitude and longitude coordinates.
- WeatherView.swift
A SwiftUI view file that lays out how weather data is presented to the user. It includes temperature, humidity, wind speed, and other relevant details.
