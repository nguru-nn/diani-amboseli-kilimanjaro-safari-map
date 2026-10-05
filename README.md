# Diani Beach → Tsavo East & Amboseli: 3-Day Kilimanjaro Safari Map
 
This is an interactive 3D map of a 3-day road safari from **Diani Beach** on Kenya's south coast. The first stop is **Tsavo East National Park**. From there the route continues to **Amboseli National Park**, where elephant herds roam with **Mount Kilimanjaro**, Africa's highest peak, as the backdrop.
 
🗺️ **See the full itinerary and the live map:**
[Safari do Amboseli i na Kilimandżaro z Diani](https://safarikenia.com.pl/safari-do-amboseli-i-na-kilimandzaro-z-diani) on **Safari Kenia**
 
---
 
## The route
 
| Day | Destination | Accommodation |
|-----|-------------|---------------|
| Start | Departure from Diani Beach | — |
| Day 1 | Tsavo East National Park | Voi Safari Lodge |
| Day 2 | Amboseli National Park, below Kilimanjaro | Amboseli Sopa Lodge |
| Day 3 | Return to Diani Beach | — |
 
**Day 1:** Diani Beach → Likoni Ferry → Mariakani → Mackinnon Road → Voi (Tsavo East)
**Day 2:** Voi → Manyani → across the Tsavo region → Amboseli
**Day 3:** Amboseli → Kimana → Emali → Mtito Andei → Mariakani → Likoni Ferry → Diani Beach
 
The route makes a loop, so the return leg uses a different road from the way out. The interface labels are in Polish, matching the tour page the map is embedded on.
 
## Features
 
- **Satellite basemap with 3D terrain.** The map uses the Mapbox Standard Satellite style with DEM terrain (1.5× exaggeration) and a tilted camera. Kilimanjaro's massif rises above the Amboseli basin, and the Chyulu Hills are visible along the way.
- **Road-accurate loop route.** Each leg is fetched from the Mapbox Directions API (driving profile) and stitched into one line. If a request fails, the map falls back to a straight segment for that leg.
- **Animated route line.** A golden "marching ants" dashed line runs over a soft glow layer.
- **Interactive itinerary panel.** A glassmorphism sidebar lists each day. Clicking a card flies the camera to that lodge and opens its popup.
- **Custom markers.** Gold SVG pins mark the overnight stops. Hidden waypoints keep the route on the correct roads.
- **Mobile-friendly.** On small screens the sidebar becomes a bottom sheet, and cooperative gestures keep page scrolling smooth.
- **WordPress-ready.** Styles are scoped to a single container, so the map can be pasted into a Custom HTML block.
## Tech stack
 
- [Mapbox GL JS](https://docs.mapbox.com/mapbox-gl-js/) v3.9.0
- [Mapbox Directions API](https://docs.mapbox.com/api/navigation/directions/)
- Vanilla JavaScript, no build step
- Plus Jakarta Sans (Google Fonts)
## Usage
 
1. Copy the HTML into a WordPress **Custom HTML** block or any web page.
2. Replace the Mapbox access token with your own, and restrict it to your domain in your [Mapbox account](https://account.mapbox.com/access-tokens/).
3. Adjust the container height in `.wp-safari-itinerary-container` to fit your layout.
To change the route, edit the `itineraryData` array. Entries with `isWaypoint: true` only shape the route. Every other entry gets a marker and a sidebar card.
 
## About
 
Built for [Safari Kenia](https://safarikenia.com.pl/), a source of Polish-language safari tours and travel guides for Kenya.
 
➡️ [View this Amboseli & Kilimanjaro safari itinerary](https://safarikenia.com.pl/safari-do-amboseli-i-na-kilimandzaro-z-diani)
 
