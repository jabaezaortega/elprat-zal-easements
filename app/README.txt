ZAL Port vs LEBL easements - static 3D web app (CesiumJS 1.147 from jsDelivr CDN, no API key / no Cesium ion).
Run locally:  cd web3d && python3 -m http.server 8000   then open http://localhost:8000  (opening index.html via file:// will not load the data because of browser fetch restrictions).
Share: zip this folder, or upload it as-is to any static host (GitHub Pages, Netlify Drop, Cloudflare Pages). Needs internet for the Cesium library and basemap tiles (OpenStreetMap / Esri World Imagery).
Data: data/envelope_mesh.json (strictest RD 657/2022 envelope, 150 m grid, m AMSL), data/zal_buildings.geojson (64 Catastro buildings with LiDAR heights and clearances), boundaries.
Heights are orthometric (m AMSL) drawn on the bare WGS84 ellipsoid (no terrain). Geoid N = +48.98 m at ZAL (EGM08-REDNAP) would have to be added if an ellipsoidal terrain were enabled.
Prototype for visual exploration only - no legal value.
