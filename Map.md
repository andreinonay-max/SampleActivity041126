<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>Regional Filipino Artist</title>

    <!-- Leaflet CSS -->
    <link rel="stylesheet"
    href="https://unpkg.com/leaflet/dist/leaflet.css"/>

    <style>

        body{
            margin:0;
            font-family: Arial, sans-serif;
        }

        h1{
            padding:15px;
        }

        #map{
            height:90vh;
            width:100%;
        }

    </style>
</head>
<body>

    <h1>Regional Filipino Artist</h1>

    <!-- MAP -->
    <div id="map"></div>

    <!-- Leaflet JS -->
    <script src="https://unpkg.com/leaflet/dist/leaflet.js"></script>

    <script>

        // CREATE MAP
        const map = L.map('map').setView([12.8797, 121.7740], 6);

        // MAP TILE
        L.tileLayer('https://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png', {
            attribution: '&copy; OpenStreetMap Contributors'
        }).addTo(map);

        // BACOLOD
        const bacolod = L.marker([10.6765, 122.9509]).addTo(map);

        bacolod.bindPopup(
            "<b>Bacolod</b><br>Charlie Co"
        );

        // LEYTE
        const leyte = L.marker([11.2440, 124.9617]).addTo(map);

        leyte.bindPopup(
            "<b>Leyte</b>"
        );

        // PANGASINAN
        const pangasinan = L.marker([15.8949, 120.2863]).addTo(map);

        pangasinan.bindPopup(
            "<b>Pangasinan</b>"
        );

    </script>

</body> 
</html>
