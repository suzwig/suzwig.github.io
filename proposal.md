---
layout: home
---

# Proposal: February 26th, 2025

I proposed to Suzie on Dickman's island, part of the Tenthousand Island Preserve near Marco Island.
I found a beautiful conch shell in the water, put the Lego ring in it and asked if she wants to marry me.

She said: "I love you!" and yes.

## Map of our Kayak Trip

<div id="map" style="width: 100%; height: 800px;"></div>

<link rel="stylesheet" href="https://unpkg.com/leaflet@1.7.1/dist/leaflet.css"
   integrity="sha512-xodZBNTC5n17Xt2atTPuE1HxjVMSvLVW9ocqUKLsCC5CXdbqCmblAshOMAS6/keqq/sMZMZ19scR4PsZChSR7A=="
   crossorigin=""/>

<script src="https://unpkg.com/leaflet@1.7.1/dist/leaflet.js"
   integrity="sha512-XQoYMqMTK8LvdxXYG3nZ448hOEQiglfqkJs1NOQV44cWnUrBc8PkAOcXy20w0vlaXaVUearIOBhiXZ5V3ynxwA=="
   crossorigin=""></script>

<script>
document.addEventListener('DOMContentLoaded', function() {
    var map = L.map('map').setView([25.90519, -81.71693], 15);

    L.tileLayer('https://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png', {
        attribution: '© OpenStreetMap contributors'
    }).addTo(map);

    L.marker([25.91258, -81.71757]).addTo(map)
        .bindPopup('Kayak Launch')

    L.marker([25.90600, -81.71622]).addTo(map)
        .bindPopup('Shelling Stop')

    L.marker([25.896675, -81.713951]).addTo(map)
        .bindPopup('Beaching the Kayak')

    L.marker([25.904335, -81.717231]).addTo(map)
        .bindPopup('Dolphins!')

    L.marker([25.89525, -81.71133]).addTo(map)
        .bindPopup('Proposal!')
        .openPopup();

    // Ensure the map renders correctly after changing its size
    map.invalidateSize();
});
</script>
