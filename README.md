# Better-Maps
Simple but flexible Maps module for FileMaker distributed in Carafe. 

This simple maps code allows most ( and soon to be more with your contributions ) Google maps feautres often needed in FileMaker web viewers. This code is a port for some pervious code to take advantage of Carafe, an open source module for code distribution for FileMaker JS modules.

## Features
- Single API interface script handles all data and configurations
- 2 way interactivity to FM so additional g=Google instantiation hits are mitigated
- simple update concept

## Overview
The main concept of BetterMaps is that you just pass the key:vales of the param syou want to update and it takes care of the rest. Want to update the markers, just pass in that array. Want to change a callback script, just pass in that key.

Refer to google maps API for more details regarding some attributes.

 Attribute  | Desctiption |
| ------------- | ------------- |
|   |   |
|   |   |
|   |   |
| `departureTimeOffset`  |  Used for calulating offset time for traffic |
|   |   |
|   |   |
| `fileName`  | FileMaker callback file name use get(filename)  |
| `setBounds`  | Will set the map bounds   |
| `showTraffic`  | Boolean - if true, will show the traffic layer  |
| `trafficModel` | Waht method will be used to calculate traffic times. Options:  `Pptinistic`, `Pesimistic`, `Best Guess`,  |
|   |   |
| `travelMode`  | 'Driving', `Transit`, `Walking`, `Bicycling`  |
|   |   |
|   |   |

| `unitSystem`  | 'metric' or imperial if not used ( default)|
