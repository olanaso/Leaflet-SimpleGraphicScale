# Simple Graphic Scale Plugin for Leaflet

This is a README file for the `SimpleGraphicScale` plugin for the Leaflet mapping library. This plugin provides a customizable, easy-to-use graphic scale control for your maps.

## Features

- Customizable position
- Option to update scale when the map is idle or not
- Configurable minimum and maximum unit widths
- Option to fill the scale with color
- Toggle subunit display
- Option for a double-line scale
- Configurable label placement
- Customizable scale color, background color, and border radius
- Optional box shadow for the scale

## Usage

First, include the plugin's CSS and JavaScript files in your HTML file:

```html
<script src="path/to/Leaflet-SImpleGraphic-Scale.js.js"></script>
```

Then, create a new `GraphicScaleSGBI` control and add it to your Leaflet map:

```javascript
var scaleControl = new L.Control.SimpleGraphicScale(options).addTo(map);
```

## Options

You can customize the behavior and appearance of the `GraphicScaleSGBI` control by providing an options object. Available options and their default values are:

```javascript
{
  position: "bottomleft",
  updateWhenIdle: false,
  minUnitWidth: 30,
  maxUnitsWidth: 240,
  fill: false,
  showSubunits: false,
  doubleLine: false,
  labelPlacement: "auto",
  color: '#fff',
  background_color_scale: 'rgba(255,255,255,0.6)',
  border_radius: '3px',
  box_shadow: true
}
```

### Options explanation

- `position`: The position of the scale control on the map. Possible values are `'topleft'`, `'topright'`, `'bottomleft'`, `'bottomright'`.
- `updateWhenIdle`: Set to `true` to update the scale only when the map is idle (not panning or zooming).
- `minUnitWidth`: The minimum width of a scale unit in pixels.
- `maxUnitsWidth`: The maximum width of all scale units in pixels.
- `fill`: Set to `true` to fill the scale with color.
- `showSubunits`: Set to `true` to display subunits on the scale.
- `doubleLine`: Set to `true` to use a double-line scale.
- `labelPlacement`: Determines the placement of scale labels. Possible values are `'auto'`, `'above'`, `'below'`, `'hide'`.
- `color`: The color of the scale labels and lines.
- `background_color_scale`: The background color of the scale control.
- `border_radius`: The border radius of the scale control.
- `box_shadow`: Set to `true` to add a box shadow to the scale control.

## License

This plugin is provided under the [MIT License](https://opensource.org/licenses/MIT).
