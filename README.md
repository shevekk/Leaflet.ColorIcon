# Leaflet.ColorIcon
Leaflet plugin for create colored icons with optional shadow.

## Screenshots
Exemple without shadow :

![ColorIcon screenshot](https://raw.github.com/shevekk/Leaflet.ColorIcon/master/screenshots/capture.png)


Exemple with shadow :

![ColorIcon shadow screenshot](https://raw.github.com/shevekk/Leaflet.ColorIcon/master/screenshots/capture_shadow.png)

<a href="http://dataexplorer.hd.free.fr/Leaflet.ColorIcon/examples/basic/" target="_blank">Demo</a> 

## Using the plugin
````xml
<script src="L.colorIcon.js"></script>
````

| Property        | Description            | Default Value | Possible  values                                     |
| --------------- | ---------------------- | ------------- | ---------------------------------------------------- |
| iconSize        | Name of the icon       | [25, 25]      | Size of the icon                                     |
| iconUrl         | Url of the icon        | ''            | Image url |
| color           | Color of the icon      | '#000000'     | Color to hex value (#ff0000) or rgb value (rgb(255, 0, 0)) |
| shadowUrl   | Url of the shadow (no shadow if empty) | ''     | Image of shadow url |
| shadowSize      | Size of the shadow     | [25, 25]    | Size of the shadow |
| shadowAnchor    | Anchor of the shadow      | [0, 0]     | The coordinates of the "tip" of the shadow (relative to its top left corner) (the same as iconAnchor if not specified). |
| shadowColor     | Color of the shadow      | '#000000'     | Color of shadow to hex value (#ff0000) or rgb value (rgb(255, 0, 0)) |

Exemple : 
````xml
let iconBuilding = L.colorIcon({
  iconSize : [30, 30],
  popupAnchor : [0, -15],
  iconUrl: "img/building-solid.svg",
  color: "#3f39b6"
});
````

Exemple with shadow : 
````xml
let iconBuildingRed = L.colorIcon({
  iconSize : [40, 40],
  popupAnchor : [0, -20],
  iconUrl: "img/building-solid.svg",
  shadowUrl: "img/building-solid.svg",
  shadowAnchor: [-3, -1],
  shadowSize: [40, 40],
  shadowColor: "#664848",
  color: "rgb(255, 0, 0)"
});
````

ColorIcon inherits from L.DivIcon, it allows to generate a css filter for create colored icon.

Your base icon image must be black to make the colorization work.

## License
Leaflet.ColorIcon is licensed under the MIT License - http://opensource.org/licenses/mit-license.html.
