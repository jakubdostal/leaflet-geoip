Leaflet.GeoIP
=============

GeoIP Plugin for Leaflet.js. This plugin allows you to find the approximate position of the client machine based on their IP address. Additionally, you can center the map on this location.


Usage
=============
Include the .js file in your html file.
```
  <script src="leaflet-geoip.js"></script>
```
Get the approximate position of the client machine as a L.LatLng object:
```
  var pos = L.GeoIP.getPosition();
```
Centre the map on the approximate location of the client machine:
```
  //initialise your map into
  //var map;

  L.GeoIP.centerMapOnPosition(map);
```
You can also do the same for the location of an arbitraty IP address:
```
  var ip = "13.15.13.15";
  var pos = L.GeoIP.getPosition(ip);
  
  //or
  
  //initialise your map into
  //var map;
  L.GeoIP.centerMapOnPosition(map, ip);
```

Credits
=============
* [freegeoip.net](http://freegeoip.net) for the free geoIP server and service ([GitHub project](https://github.com/fiorix/freegeoip))
