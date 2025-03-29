# Weather App

A web-based weather application that provides real-time weather information for cities worldwide using the OpenWeatherMap API. This project was developed as part of the "Playing Around with APIs" assignment.

## Table of Contents
- [Overview](#overview)
- [Features](#features)
- [Technologies Used](#technologies-used)
- [API Integration](#api-integration)
- [Deployment](#deployment)
- [Challenges and Solutions](#challenges-and-solutions)
- [Demo](#demo)
- [Credits](#credits)

## Overview

This application serves a practical purpose by providing users with accurate, up-to-date weather information for any city in the world. Users can quickly search for weather conditions, view current temperatures, and access additional meteorological data such as humidity, wind speed, and atmospheric pressure.

## Features

- **City-based Weather Search**: Users can search for weather information by entering city names
- **Real-time Data**: Displays current weather conditions pulled from OpenWeatherMap API
- **Comprehensive Weather Details**: Shows temperature, feels-like temperature, humidity, wind speed, and pressure
- **Visual Weather Indicators**: Includes weather icons representing current conditions
- **Responsive Design**: Works seamlessly across desktop and mobile devices
- **User-friendly Interface**: Clean, intuitive design for easy navigation and use
- **Error Handling**: Provides helpful feedback when cities cannot be found or when API errors occur

## Technologies Used

- HTML5
- CSS3
- JavaScript (ES6+)
- Fetch API for asynchronous requests
- OpenWeatherMap API

## API Integration

This project utilizes the [OpenWeatherMap API](https://openweathermap.org/api), a comprehensive weather data service that provides:

- Current weather data
- Weather forecasts
- Historical weather data
- Weather maps

The application makes use of the Current Weather Data endpoint, which returns real-time weather information based on city name. The API responses are processed and displayed in a user-friendly format.

## Deployment

The application has been deployed to two web servers (Web01 and Web02) with a load balancer (Lb01) distributing traffic between them.


## Challenges and Solutions

### Challenge 1: API Rate Limiting
**Solution:** Implemented client-side caching to store weather data temporarily, reducing the number of API calls for frequently searched cities.

### Challenge 2: Load Balancer Session Persistence
**Solution:** Configured cookie-based session persistence to ensure users consistently connect to the same backend server during their session.

### Challenge 3: Secure API Key Management
**Solution:** Implemented environment variables on the server side to securely store API keys, preventing exposure in client-side code.

## Demo

A short demonstration video showing the application's functionality and deployment can be found here: [Demo Video Link]()

The video covers:
- How to use the application to search for weather information
- The application's response and data display
- Accessing the application through the load balancer
- Verification of load balancing functionality

## Credits

- Weather data provided by [OpenWeatherMap API](https://openweathermap.org/api)
- Weather icons from OpenWeatherMap
- HTML/CSS/JavaScript implementation by Igornoel
- A help of AI to formalize my code

---

*This project was created as an assignment for Web Infrastructure. For questions or feedback, please contact n.ishimwe4@alustudent.com.*
