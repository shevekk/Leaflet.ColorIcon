# Leaflet.ColorIcon
Leaflet plugin for create colored icons

## Screenshots
![ColorIcon screenshot](https://github.com/shevekk/Leaflet.ColorIcon/tree/main/screenshots/capture.png)

<a href="http://dataexplorer.hd.free.fr/Leaflet.ColorIcon/examples/basic/" target="_blank">Demo</a> 

## Using the plugin
````xml
<script src="L.colorIcon.js"></script>
````

| Property        | Description            | Default Value | Possible  values                                     |
| --------------- | ---------------------- | ------------- | ---------------------------------------------------- |
| iconSize        | Name of the icon       | 'home'        | Size of the icon                                     |
| iconUrl         | Url of the icon        | ''            | Your image |
| color           | Color of the icon      | '#000000'     | Color to hex value (#ff0000) or rgb value (rgb(255, 0, 0)) |

Exemple : 
````xml
let iconBuilding = L.colorIcon({
  iconSize : [30, 30],
  popupAnchor : [0, -15],
  iconUrl: "img/building-solid.svg",
  color: "#3f39b6"
});
````
