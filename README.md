# openlayers-draw-toolbar-control

## Installation

This assumes you have Openlayers installed. Add file to prefered location and import it into the file where your map variable is instantiated.

## Usage

```typescript
import {drawTools} from './MapControls.js';

const olMap = new Map({
  controls: defaultControls().extend([new ScaleLine(), new FullScreen(), new drawTools({layer: vector,drawTypes:['Polygon','Circle','Line','Point'],top:5.5,left:.5})]),
  layers: [
    
    new TileLayer({
      source: new OSM()
    }),
    vector
  ],
  view: new View({
    center: [-357509.106, 7256652.10], 
    zoom: 10
  })

});
```
Change constructor as required.
![Image of drawTool](https://github.com/Dev-Boshoff/openlayers-draw-toolbar-control/drawTool.png)

