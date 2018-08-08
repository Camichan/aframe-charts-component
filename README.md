## aframe-charts-component

[![Version](http://img.shields.io/npm/v/aframe-charts-component.svg?style=flat-square)](https://npmjs.org/package/aframe-charts-component)
[![License](http://img.shields.io/npm/l/aframe-charts-component.svg?style=flat-square)](https://npmjs.org/package/aframe-charts-component)

Make 3D Charts with this component based on [A-Frame](https://aframe.io).

### API

| Property | Description | Default Value |
| -------- | ----------- | ------------- |
| dataPoints | Path to JSON input data |  ../data/data.json  |
| type         | Chart type. Currently we have bubble, bar and cylinder charts            |  bubble             |

### JSON File
We need this file wich contains the points in order to generate the chart. The path of this file must be included in dataPoint property.

Example JSON file:

```json
[
  {"x": 1, "y": 8, "z": 0, "size": 1, "color": "#ff0000"},
  {"x": -2, "y": 3, "z": 1, "size": 1.5, "color": "#00ff00"},
  {"x": -1, "y": 3, "z": 2, "size": 1, "color": "#0000ff"},
  {"x": 2, "y": 7, "z": 7, "size": 1.5, "color": "#0000ff"},
  {"x": 1, "y": 6, "z": 3, "size": 1, "color": "#4CC3D9"}
]  
```


### Installation

#### Browser

Install and use by directly including the [browser files](dist):

```html
<head>
  <title>My A-Frame Scene</title>
  <script src="https://aframe.io/releases/0.8.2/aframe.min.js"></script>
  <script src="https://unpkg.com/aframe-charts-component/dist/aframe-charts-component.min.js"></script>
</head>

<body>
  <a-scene>
    <a-entity charts="dataPoints: ../data/data.json; type: bar"></a-entity>
  </a-scene>
</body>
```

#### npm

Install via npm:

```bash
npm install aframe-charts-component
```

Then require and use.

```js
require('aframe');
require('aframe-charts-component');
```
