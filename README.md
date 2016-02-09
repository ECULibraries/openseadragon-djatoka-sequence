# openseadragon-djatoka-sequence
Implementation of [OpenSeadragon](https://github.com/openseadragon/openseadragon) that displays a sequence of images using Islandora's [Djatoka TileSource](https://github.com/Islandora/islandora_openseadragon/blob/7.x/js/djtilesource.js).

### Instructions
Add source images to tiles array and set djatokaBaseUrl.
```javascript
var tiles = ["FILE1.JP2", "FILE2.JP2"];
             
OpenSeadragon({
   id: "viewer",
   prefixUrl: "images/",
   tileSources: tiles,
   djatokaBaseUrl: "http://localhost:8080/adore-djatoka",
   djatokaSettings: {tileSize: 256, tileOverlap: 0},
   sequenceMode: true,
   showRotationControl: true
});
```
