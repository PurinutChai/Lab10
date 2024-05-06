# Lab10
งาน Lab10
<!DOCTYPE html>
<html>
<head>
<title> Creating Maps with Leaflet </title>
<link rel="stylesheet" href=https://unpkg.com/leaflet@1.9.3/dist/leaflet.css integrity="sha256-kLaT2GOSpHechhsozzB+flnD+zUyjE2LlfWPgU04xyI="crossorigin=""/>
<script src=https://unpkg.com/leaflet@1.9.3/dist/leaflet.js integrity="sha256-WBkoXOwTeyKclOHuWtc+i2uENFpDZ9YPdf5Hf+D7ewM=" crossorigin=""></script>

</head>
<body>
<div id="map" style="height: 600px"> </div>
<script>
var map = L.map('map').setView([13.7563, 100.5018], 10);
L.tileLayer('http://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png', {
    attribution: '&copy; <a href="http://osm.org/copyright">OpenStreetMap</a> contributors'
}).addTo(map);
var greenIcon = L.icon({
iconUrl: 'pin.png',
iconSize:     [30, 30], // size of the icon
iconAnchor:   [45, 45], // point of the icon which will correspond to marker's location
popupAnchor:  [0, -39] // point from which the popup should open relative to the iconAnchor		
});


L.marker([13.75018, 100.49188],{icon:greenIcon}).addTo(map).bindPopup("<b>The Grand Palace</b><br>Pranakorn district, Bangkok<br>");
L.marker([13.72669, 100.51034],{icon:greenIcon}).addTo(map).bindPopup("<b>Iconsiam</b><br>Khlong San district, Bangkok<br>");
L.marker([13.74678, 100.53499],{icon:greenIcon}).addTo(map).bindPopup("<b>Siam Paragon</b><br>Pathumwan district, Bangkok<br>");
L.marker([13.70417, 100.50290],{icon:greenIcon}).addTo(map).bindPopup("<b>Asiatique</b><br>Bang Kho Laem district, Bangkok<br>");
L.marker([13.98936, 100.61825],{icon:greenIcon}).addTo(map).bindPopup("<b>Future Park Rangsit</b><br>Thanyaburi district, Pathum Thani<br>");
L.marker([13.74632, 100.49285],{icon:greenIcon}).addTo(map).bindPopup("<b>Wat Arun Ratchawararam</b><br>Bangkok Yai district, Bangkok<br>");
L.marker([13.91806, 100.54735],{icon:greenIcon}).addTo(map).bindPopup("<b>Thunderdome Stadium</b><br>Pak Kret district, Nonthaburi<br>");
L.marker([13.86552, 100.70343],{icon:greenIcon}).addTo(map).bindPopup("<b>Safari World</b><br>Khlong Sam Wa district, Bangkok<br>");



</script>
</body>
</html>
