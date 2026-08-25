Operation Vijay — Real Satellite Build V3

Run locally:
1. Extract the ZIP.
2. Start a local web server in the extracted folder, for example:
   python -m http.server 8000
3. Open:
   http://localhost:8000/operation-vijay-real-satellite-v2.html

New in V4:
- Integrates the uploaded Dassault Mirage 2000 3D model.
- Integrates the uploaded MiG-21 Bison 3D model.
- Mirage appears during the precision-strike story beat.
- MiG-21 appears during the later air-operation story beat.
- Models are centered and normalized automatically.
- Actual model flight paths replace the previous generic low-poly jet.
- Perspective switching is now handled through explicit pointer and click handlers.
- Camera blends start from the actual smoothed camera state and finish exactly on the selected path.
- Added a global switchPerspective(key) entry point for easy debugging.
- Original model texture folders and license files are preserved under assets/.

Note:
- The page loads Three.js and GLTFLoader from CDNs, so internet access is needed
  unless those scripts are later bundled locally.
- Serve the project through a local HTTP server; opening the HTML directly via
  file:// may block model and texture loading in some browsers.
