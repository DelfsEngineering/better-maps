# Better-Maps
Simple but flexible Maps module for FileMaker distributed in Carafe.

This simple maps code allows most (and soon even more with your contributions) Google Maps features often needed in FileMaker web viewers. This code is a port from some previous work and leverages Carafe, an open source module for distributing FileMaker JavaScript modules.

## Features
- Single API interface script handles all data and configurations
- Two-way interactivity with FileMaker reduces additional Google instantiation hits
- Simple update mechanism

## Overview
The main concept of BetterMaps is that you pass the key/value pairs for the parameters you want to update and it takes care of the rest. Want to update the markers? Just pass that array. Need to change a callback script? Simply pass in that key.

Refer to Google Maps API for more details regarding some attributes.

 Attribute  | Value | Description |
| ------------- |------------- | ------------- |
| departureTimeOffset  | |  Used for calculating offset time for traffic in ms from now |
| fileName  | | FileMaker callback file name use Get(FileName) required for callbacks, only needs to be set once.  |
| mapBorderArray |  |If set, this array will be used to draw the map border |
| mapCenter |  |Centers map on passed `location` |
| cluster |  | Boolean - If true, hides markers and shows clusters |
| markersArray |  |If set, this array of marker objects will be drawn on the map |
| neighborhoodBorderArray |  |If set, a neighborhood array (outline) will be drawn |
| optimizeWaypoints | true | If true, the routes will be optimized |
| routesArray |  |If set, this array will be passed in as an array of routes for multi-route routing.|
| scriptDirectionResults |  |Script name to call back when the directions/routing returns from Google |
| scriptSendCoordinatesToFM | | Script name to call back when sending coordinates back to FileMaker, if not set, no callback is performed. Coordinates are sent on events such as map move and zoom change.|
| scriptSendGeoToFM |  | Script name to call back when the map is clicked |
| setBounds  |  | Will set the map bounds
| showDirectionsPanel |  | Boolean - if true the sidebar shows the direction results |
| showInfoWindow |  | Shows marker info window for passed `id` |
| showTraffic  |  | Boolean - if true, shows the traffic layer  |
| travelMode  |  | Type of transportation for calculating routes. Options: `Driving`, `Transit`, `Walking`, `Bicycling`  |
| trafficModel |  | What method will be used to calculate traffic times. Options:  `Optimistic`, `Pessimistic`, `Best Guess`,  |
| unitSystem  | | `metric` or `imperial` if not specified (default)|
| mapZoom |  | Map zoom level, 1-19 |
