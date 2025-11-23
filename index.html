<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />

    <!-- leaflet css link  -->
    <link
      rel="stylesheet"
      href="https://unpkg.com/leaflet@1.7.1/dist/leaflet.css"
    />

    <title>Web-GIS with geoserver and leaflet</title>

    <style>
      body {
        margin: 0;
        padding: 0;
      }
      #map {
        width: 100%;
        height: 100vh;
      }
    </style>
  </head>
  <body>
    <div id="map"></div>

<!-- leaflet js link  -->
<script src="https://unpkg.com/leaflet@1.7.1/dist/leaflet.js"></script>

<!-- jquery link  -->
<script src="https://cdnjs.cloudflare.com/ajax/libs/jquery/3.5.1/jquery.min.js"></script>

<!-- leaflet geoserver request link  -->
<script src="https://cdn.jsdelivr.net/npm/leaflet-geoserver-request@1.3.0/src/L.Geoserver.min.js"></script>

<script src="lib/L.Geoserver.js"></script>

<script>
// Inisialisasi peta
var map = L.map("map").setView([-7.677567, 110.406899], 12);

// Base map OSM
var osm = L.tileLayer("https://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png", {
    maxZoom: 19,
    attribution: '&copy; <a href="https://www.openstreetmap.org/copyright">OpenStreetMap</a> contributors',
});
osm.addTo(map);

// ==========================
// WMS GEOSERVER
// ==========================

// Layer 1 — Batas Administrasi Desa
var wmsLayer1 = L.Geoserver.wms("http://localhost:8080/geoserver/wms", {
    layers: "pgw:Batas_Admin_Sleman",
    transparent: true,
});
wmsLayer1.addTo(map);

// Layer 2 — Jalan (contoh memakai Sleman geoportal)
var wmsLayer2 = L.Geoserver.wms("https://geoportal.slemankab.go.id/geoserver/wms", {
    layers: "geonode:jalan_kabupaten_sleman_2023",
    transparent: true,
});
wmsLayer2.addTo(map);

// Layer 3 — Penduduk Sleman
var wmsLayer3 = L.Geoserver.wms("http://localhost:8080/geoserver/wms", {
    layers: "pgw:Penduduk_sleman_view",
    transparent: true,
});
wmsLayer3.addTo(map);

// ==========================
// LEGEND WMS
// ==========================
var layerLegend = L.Geoserver.legend("http://localhost:8080/geoserver/wms", {
    layers: "pgw:Batas_Admin_Sleman",
});
layerLegend.addTo(map);

// ==========================
// LAYER CONTROL
// ==========================
var baseMaps = {
    "OpenStreetMap": osm
};

var overlayMaps = {
    "Batas Administrasi Desa": wmsLayer1,
    "Jalan": wmsLayer2,
    "Penduduk": wmsLayer3
};

var layerControl = L.control.layers(baseMaps, overlayMaps).addTo(map);

</script>
