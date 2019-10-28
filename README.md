# Better-Maps
Simple but flexible Maps module for FileMaker distributed in Carafe. 

This simple maps code allows most ( and soon to be more with your contributions ) Google maps feautres often needed in FileMaker web viewers. This code is a port from some pervious code to take advantage of Carafe, an open source module for code distribution for FileMaker JS modules.

## Features
- Single API interface script handles all data and configurations
- 2 way interactivity to FM so additional Google instantiation hits are mitigated
- simple update concept

## Overview
The main concept of BetterMaps is that you just pass the key:vales of the param syou want to update and it takes care of the rest. Want to update the markers, just pass in that array. Want to change a callback script, just pass in that key.

Refer to google maps API for more details regarding some attributes.

 Attribute  | Value | Description |
| ------------- |------------- | ------------- |
| departureTimeOffset  | |  Used for calulating offset time for traffic |
| fileName  |  |FileMaker callback file name use get(filename) required for callbacks, only needs to be set once.  |
| mapBorderArray |  |If set, this array will be used to draw the map boarder |
| mapCenter |  |Centers map on passed `location` |
| markersArray | I |f set, thei array of marker objects will be drawn on the map |
| neighborhoodBorderArray |  |If set, an neabourhood array ( outline) will be drawn |
| routesArray |  |If set, this array will be passed in as an array of routes for multi-route ruoting.|
| scriptDirectionResults |  |Script name to callback to when the directions/routing has returned from Google |
| scriptSendCoordinatesToFM | | Script name to callback to when sending coordinates back to FM, if not set, no callback in performed. Coords are sen on things like mamp move and zoom change.|
| scriptSendGeoToFM |  | Script name to callback to when the map is clicked |
| setBounds  |  | Will set the map bounds   |\
| showDirectionsPanel |  | Boolean, if true the sidebar will show the direction results |
| showInfoWindow |  | Shows marking info window for passed `id` |
| showTraffic  |  | Boolean - if true, will show the traffic layer  |
| travelMode  |  | Type of transportation for calculating routes. Options: `Driving`, `Transit`, `Walking`, `Bicycling`  |
| trafficModel |  | What method will be used to calculate traffic times. Options:  `Pptinistic`, `Pesimistic`, `Best Guess`,  |
| unitSystem  | | `metric` or imperial if not used ( default)|
| mapZoom |  | Map zoom level, 1-19? |
