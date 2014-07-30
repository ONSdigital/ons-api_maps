ONS Geography API Example
============
 
This demo is built using HTML and JavaScript and should work on any modern web browser.
 
The ONS Open Geography service makes many products available to the public including all the administrative boundaries used with ONS data. These can be discovered using the public API. For simplicity, this demo uses a single vector boundary set, 2011 Wards. The Open Geography API has a function to find areas matching on name or code. This demo does such a find based on the contents of a text box. The boundaries of the first matching ward are then retrieved (and the name of the first match reported, see screen shot below) via JSONP. In order to plot the boundary on Google Maps, the points have to be converted from Easting / Northing to Latitude / Longitude. This is done using a slightly inaccurate formula. A JavaScript array containing the points is then presented to the Google Maps API, with the map centred and zoomed by working out the minimum and maximum latitude and longitude.
 
Data records returned from the ONS API will always have the standard area code present, so this is the way to link data and maps.

![Screenshot](https://raw.githubusercontent.com/ONSdigital/ons-api_maps/master/screenshot.jpg "Screenshot")
