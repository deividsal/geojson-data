# GeoJSON Live Data Map

This project demonstrates how to render live, real-time geospatial data on an interactive web map. The included example displays the last 24 hours of earthquake activity from the United States Geological Survey (USGS) on top of an OpenStreetMap base layer using [Leaflet](https://leafletjs.com/).

## Getting started

1. Serve the contents of this directory using any static file server. For example:

   ```bash
   npx serve .
   ```

2. Open `http://localhost:3000` (or whichever port your server reports) in your browser.

3. The map will automatically retrieve the most recent earthquake data from the USGS GeoJSON feed and plot it on the map. Markers are colored and sized according to magnitude, and clicking on a marker reveals more information.

## Customising the data source

To visualise a different live GeoJSON feed:

1. Update the `feedUrl` constant in `index.html` with the new endpoint.
2. Adjust the popup template and any styling logic in the script to match the structure of your data.

A sample static `data.geojson` file is also included to illustrate the expected GeoJSON structure if you want to serve your own dataset.

## Credits

- Base map tiles &copy; [OpenStreetMap](https://www.openstreetmap.org/) contributors
- Earthquake data &copy; [USGS Earthquake Hazards Program](https://earthquake.usgs.gov/)
