<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Philippines Map</title>

    <link rel="stylesheet"
    href="https://unpkg.com/leaflet/dist/leaflet.css"/>

    <style>

        body{
            margin:0;
            font-family:Arial;
        }

        h1{
            text-align:center;
            padding:10px;
        }

        #map{
            height:90vh;
            width:100%;
        }

    </style>
</head>
<body>

<h1>Regional Filipino Artists</h1>

<div id="map"></div>

<script src="https://unpkg.com/leaflet/dist/leaflet.js"></script>

<script>

const map = L.map('map').setView([12.8797,121.7740],6);

L.tileLayer('https://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png',{
    attribution:'&copy; OpenStreetMap Contributors'
}).addTo(map);

// Bacolod
L.marker([10.6765,122.9509])
.addTo(map)
.bindPopup("<b>Bacolod</b><br>Charlie Co");

// Leyte
L.marker([11.2440,124.9617])
.addTo(map)
.bindPopup("<b>Leyte</b>");

// Pangasinan
L.marker([15.8949,120.2863])
.addTo(map)
.bindPopup("<b>Pangasinan</b>");

</script>

</body>
</html>

</body>
</html>
