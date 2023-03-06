# Project Name

**Author**: Deon Curry
**Version**: 1.0.0 (increment the patch/fix version number if you make more commits past your first submission)

## Overview

This is a web application that allows users to search for a city and get information about the location such as a map, images, and weather.


## Getting Started

To use this application, enter the name of the city you want to search for in the search bar and click the "Explore!" button. The app will then display a map of the location, photos of the city, and the current weather information for that location.


## Architecture

The user enters a city name in the search bar and clicks the "Explore!" button.

The handleSubmit function in App.js is called, which sends a request to the LocationIQ API with the entered city name as a query parameter.

The LocationIQ API returns a response with the latitude and longitude of the location.

The handleSubmit function then sends a request to the backend server with the latitude and longitude as query parameters.

The server then sends requests to the Open Weather Map API and the Pexels API for weather and photo data respectively.

The Open Weather Map API and the Pexels API both return responses with the requested data.

The server combines the data from both APIs and sends a response back to the handleSubmit function.

The handleSubmit function sets the state variables for the map, photos, and weather data with the received data.

The render function then updates the UI with the received data.
Functions

handleSubmit: This function is called when the user submits the search form. It sends a request to the LocationIQ API to get the latitude and longitude of the entered city. It then sends a request to the backend server with the 
latitude and longitude as query parameters.
getMap: This function takes latitude and longitude as parameters and returns a URL to a map of the location using the Mapbox API.
getWeather: This function takes latitude and longitude as parameters and returns weather data for that location from the Open Weather Map API.
getPhotos: This function takes a city name as a parameter and returns photos of that location from the Pexels API.
server.js: This file contains the backend server that handles requests from the frontend and communicates with the Open Weather Map and Pexels APIs to get weather and photo data respectively.
Dependencies
Axios
Bootstrap
Environment Variables
REACT_APP_LOCATIONIQ_API_KEY: API key for the LocationIQ API
REACT_APP_BACKEND_URL: URL for the backend server
Netlify Deployment
This app has been deployed to Netlify at https://city-explorer.netlify.app/.


## Change Log

## Credit and Collaborations


Name of feature: ________._______________________

Estimate of time needed to complete: __5___

Start time: __1330___

Finish time: _____

Actual time needed to complete: _____