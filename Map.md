<link rel="stylesheet"
href="https://unpkg.com/leaflet/dist/leaflet.css"/> 
<script src="https://unpkg.com/leaflet/dist/leaflet.js"></script>
<script src="map.js"></script> 

// Create map
const map = L.map('map').setView([12.8797, 121.7740], 6);

// Map tiles
L.tileLayer('https://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png', {
    attribution: '&copy; OpenStreetMap Contributors'
}).addTo(map);

// BACOLOD
const bacolod = L.marker([10.6765, 122.9509]).addTo(map);

bacolod.bindPopup("<b>Bacolod</b><br>Charlie Co");

// LEYTE
const leyte = L.marker([11.2440, 124.9617]).addTo(map);

leyte.bindPopup("<b>Leyte</b>");

// PANGASINAN
const pangasinan = L.marker([15.8949, 120.2863]).addTo(map);

pangasinan.bindPopup("<b>Pangasinan</b>");

<div id="map"></div> 
#map{
    height: 600px;
    width: 100%;
} 
git add .
git commit -m "Added map markers"
git push 
