# india-aqi-live
India Air Quality Live
A single-page web app that shows real-time air quality for 20 Indian cities on an interactive map.
Live demo: https://navya01106.github.io/india-aqi-live/
<!-- Add a screenshot: upload it to the repo and use ![Screenshot](screenshot.png) -->
Features
Live AQI, PM2.5 and PM10 for 20 cities, fetched in a single API request
Interactive map where circle size and colour scale with air quality
Cities ranked from worst to best air; click a city to zoom to it
Six-level AQI scale with a short health tip for each level
Alert banner when any city's air is unhealthy (AQI above 150)
Auto-refresh every 10 minutes
Responsive layout with light and dark mode
How it works
fetch() calls the Open-Meteo Air Quality API with all city coordinates at once.
Each city's latitude and longitude are placed on a Leaflet.js map as a circle marker.
The AQI value picks the colour, size and health tip.
setInterval polls the API every 10 minutes to keep the data fresh.
Tech
JavaScript (async/await, DOM), Leaflet.js, OpenStreetMap tiles, Open-Meteo Air Quality API. No build step and no API key needed.
Run locally
Download index.html and open it in a browser.
Data note
Values come from Open-Meteo's modelled estimates and use the US AQI scale. They are not the official CPCB (India) index and are not medical advice.
Ideas for next steps
24-hour history chart per city
City search and "use my location"
Hindi/English toggle
About this project
Built with AI-assisted coding tools. I handled the concept, design decisions, testing and deployment.
