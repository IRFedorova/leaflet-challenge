# leaflet-challenge
Import & Visualize the Data
Create a map using Leaflet that plots all of the earthquakes from your data set based on their longitude and latitude.

The goal of the project is to display multiple and interactive maps with the location and magnitude of earthquakes during the last 7 days around the world. 
The Javascript-Leaflet library, HTML, CSS, Bootstrap, and Javascript were used in the project. The Mapbox-API was also used to load the base maps. 

The project was divided into two steps with different levels of complexity.

Step 1: A single base layer and one set of data were used:

Base layer: mapbox.streets-basic
Data layer Source and Data:
Source: United States Geological Survey (USGS)
Data: Earthquakes - All Earthquakes for the last 7 days

Step 2: Multiple optional and interactive base layers were included. 
An additional dataset and plot were included and they can be activated and deactivated by the user.

Base layer:
mapbox.greyscale
mapbox.satellite
mapbox.outdoors

Data layer Source and Data:
Layer 1 Earthquake information
Source: United States Geological Survey (USGS)

Data: Earthquakes - Last 7 days - All Earthquakes)
Layer 2: Tectonic Plates
Source: Hugo Ahlenius, GIS-and-Cartography Consultant

Data: Tectonic Plates Boundaries
Libraries Required (already included in the index.html file)
D3 JavaScript
Leaflet

Sample app Screenshot
Step 1:
Screenshot

Step 2:
Screenshot

Instructions
Steps
Download or clone all the files contained in this repo.
Create a Mapbox Token
Include your Mapbox Token in the /Leaflet-Step-1/static/js/config.js and /Leaflet-Step-2/static/js/config.js files.
Run a python -m http.server or any other method for this purpose.
Load the Leaflet-Step-1/index.html and Leaflet-Step-2/index.html files.

File Description
Leaflet-Step-1
It contains all the files for the first part of the project.
index.html
Contains the HTML code that drives the maps and references the required libraries
static
It contains the CSS file with the formatting information
It contains the js with the Javascript code using the D3 library for the interactive plots.
Screenshots
It contains the gif and png files with screenshots of the app running
Leaflet-Step-2
It contains all the files for the second part of the project.
All folder are the same with this exception:
static (2)
It contains an additional folder that contains the JSON file with the tectonic-plate-boundaries information
Your first task is to visualize an earthquake data set.


Get your data set

The USGS provides earthquake data in a number of different formats, updated every 5 minutes. 
Visit the USGS GeoJSON Feed page and pick a data set to visualize. 
When you click on a data set, for example 'All Earthquakes from the Past 7 Days', you will be given a JSON representation of that data. 
You will be using the URL of this JSON to pull in the data for our visualization.



data markers reflects the magnitude of the earthquake by their size and and depth of the earth quake by color. 
Earthquakes with higher magnitudes should appear larger and earthquakes with greater depth should appear darker in color.

the map includes popups that provide additional information about the earthquake when a marker is clicked.


Legend created that will provide context for the map data.


Level 2: More Data 
The USGS wants you to plot a second data set on your map to illustrate the relationship between tectonic plates and seismic activity. 
You will need to pull in a second data set and visualize it along side your original set of data. 
Data on tectonic plates can be found at https://github.com/fraxen/tectonicplates.


Add layer controls to our map.



