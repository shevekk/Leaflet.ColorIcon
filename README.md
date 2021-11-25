# Leaflet.ColorIcon
Leaflet plugin for create colored icons

## Screenshots
![ColorIcon screenshot](https://raw.github.com/shevekk/Leaflet.ColorIcon/master/screenshots/capture.png)

<a href="http://dataexplorer.hd.free.fr/Leaflet.ColorIcon/examples/basic/" target="_blank">Demo</a> 

## Using the plugin
````xml
<script src="L.colorIcon.js"></script>
````

| Property        | Description            | Default Value | Possible  values                                     |
| --------------- | ---------------------- | ------------- | ---------------------------------------------------- |
| iconSize        | Name of the icon       | [25, 25]      | Size of the icon                                     |
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

ColorIcon inherits from L.DivIcon, it allows to generate a css filter for create colored icon

## License
Leaflet.ColorIcon is licensed under the MIT License - http://opensource.org/licenses/mit-license.html.
