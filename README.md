# GIS_PK1st4
My first website on GIS expertise
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>GIS Tutorials</title>
    <link rel="stylesheet" href="style.css">
    <link rel="stylesheet" href="https://unpkg.com/leaflet/dist/leaflet.css" />
</head>
<body>
    <header>
        <h1>Welcome to GIS Tutorials</h1>
        <nav>
            <a href="index.html">Home</a>
            <a href="tutorials.html">Tutorials</a>
            <a href="#contact">Contact</a>
        </nav>
    </header>

    <section>
        <h2>Learn GIS with Interactive Maps</h2>
        <p>Explore our tutorials to understand GIS and mapping technologies.</p>
        
        <div id="map"></div> <!-- Interactive Map -->
    </section>

    <footer id="contact">
        <p>Contact: gis.tutorial@example.com</p>
    </footer>

    <script src="https://unpkg.com/leaflet/dist/leaflet.js"></script>
    <script src="script.js"></script>
</body>
</html>
body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
    text-align: center;
}

header {
    background: #0078A8;
    color: white;
    padding: 10px 0;
}

nav a {
    margin: 0 15px;
    color: white;
    text-decoration: none;
    font-weight: bold;
}

#map {
    height: 400px;
    width: 80%;
    margin: 20px auto;
    border: 2px solid #ddd;
}

footer {
    background: #0078A8;
    color: white;
    padding: 10px 0;
    margin-top: 20px;
}
document.addEventListener("DOMContentLoaded", function() {
    var map = L.map('map').setView([23.8103, 90.4125], 6); // Centered on Bangladesh

    L.tileLayer('https://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png', {
        attribution: '&copy; OpenStreetMap contributors'
    }).addTo(map);
    
    L.marker([23.8103, 90.4125]).addTo(map)
        .bindPopup("Welcome to GIS Tutorials!")
        .openPopup();
});
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>GIS Tutorials</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <header>
        <h1>GIS Tutorials</h1>
        <nav>
            <a href="index.html">Home</a>
            <a href="tutorials.html">Tutorials</a>
            <a href="index.html#contact">Contact</a>
        </nav>
    </header>

    <section>
        <h2>Introduction to GIS</h2>
        <p>GIS (Geographic Information System) helps visualize, analyze, and interpret spatial data.</p>
        
        <h3>Basic GIS Concepts</h3>
        <ul>
            <li>What is GIS?</li>
            <li>Types of GIS Data (Raster vs. Vector)</li>
            <li>How to Use GIS for Mapping</li>
        </ul>

        <h3>Interactive Mapping with Leaflet.js</h3>
        <p>Use JavaScript and Leaflet.js to create interactive maps.</p>
    </section>

    <footer>
        <p>Contact: gis.tutorial@example.com</p>
    </footer>
</body>
</html>
# GIS Tutorials Website

This is a simple GIS tutorial website hosted on GitHub Pages. It includes:
- An interactive map using Leaflet.js
- Basic GIS learning materials
- Tutorials on GIS concepts

