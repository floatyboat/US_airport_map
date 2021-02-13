# Map of US Airports

## Introduction
This project was made to map the airports in all 50 US states, Washington D.C., and Puerto Rico. The chloropleth shown on the map displays the differences in the amount of airports state-by-state. Each airport is also labeled according to the existence of an air traffic control tower on the premises.

## Major Functions
   - airports Functions
     - onEachFeature - applies an interactive popup to the airport marker that displays the airport name when clicked
     - pointToLayer - applies the font awesome style to the marker and the color according to the precense of an air traffic control towers
   - setColor - sets the color of the state polygon according to the number of airports the state has
   - style - sets the style for the state polygon, including a call to setColor
   - legend function - adds the HTML DOM elements for the legend when it is added to the map

## Libraries
- [Leaflet](https://leafletjs.com/)
  - JS and CSS library used to create and style the map objects
- [Font Awesome](https://fontawesome.com/)
  - CSS library used to style the icons
- [Chroma](https://gka.github.io/chroma.js/)
  - JS library used to create the color pattern for the chloropleth map

## Data
- airports.geojson
  - from [data.gov](https://catalog.data.gov/dataset/usgs-small-scale-dataset-airports-of-the-united-states-201207-shapefile)
  - shapefile unzipped and converted to geoJSON
  - contains the location of the airports
  - contains the data on the precense of an air traffic control tower at each airport
- us-states.geojson
  - from [D3](http://d3js.org/) courtesy of [Mike Bostock](http://bost.ocks.org/mike)
  - geojson data file
  - contains the polygons used to make the state chloropleth
  - contains the count of airports in each state

## Basemap
Courtesy of [CartoDB](https://carto.com/)
