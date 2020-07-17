# js
a build of Mapbox GL JS

# To use
```html
<!doctype html>
<html>
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title></title>
<link rel="stylesheet" type="text/css" href="https://unvt.github.io/js/mapbox-gl.css">
<style>
body { margin: 0; top: 0; bottom: 0; width: 100%; }
#map { position: absolute; top: 0; bottom: 0; width: 100%; }
</style>
<script src="https://unvt.github.io/js/mapbox-gl.js"></script>
</head>
<body>
  <div id="map"></div>
  <script type="module">
  const map = new mapboxgl.Map({
    container: 'map',
    style: 'https://example.com/somewhere/style.json',
    attributionControl: true,
    hash: true
  })

  map.addControl(new mapboxgl.NavigationControl())
  map.addControl(new mapboxgl.ScaleControl({
    maxWidth: 200, unit: 'metric'
  }))
  </script>
</body>
</html>
```

# To update
```zsh
rake
git add .
git commit -m update
git push origin master
```
