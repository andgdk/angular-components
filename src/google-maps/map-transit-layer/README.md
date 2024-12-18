# MapTransitLayer

The `MapTransitLayer` component wraps the [`google.maps.TransitLayer` class](https://developers.google.com/maps/documentation/javascript/reference/map#TransitLayer) from the Google Maps JavaScript API.

## Example

```typescript
// google-maps-demo.component.ts
import {Component} from '@angular/core';
import {GoogleMap, MapTransitLayer} from '@angular/google-maps';

@Component({
  selector: 'google-map-demo',
  templateUrl: 'google-map-demo.html',
  imports: [GoogleMap, MapTransitLayer],
})
export class GoogleMapDemo {
  center: google.maps.LatLngLiteral = {lat: 24, lng: 12};
  zoom = 4;
}
```

```html
<!-- google-maps-demo.component.html -->
<google-map height="400px" width="750px" [center]="center" [zoom]="zoom">
  <map-transit-layer />
</google-map>
```
