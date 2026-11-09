# Madeira Webcams

One page with a map of Madeira and live webcams for Porto Moniz, Calheta, Ponta do Sol, Ribeira Brava, Câmara de Lobos, Praia Formosa, Funchal Pontinha, Reis Magos, Santa Cruz and Machico. Click a pin or a name to play the stream.

Live: https://roel-heremans.github.io/MadeiraWebcams-Site/

- Everything is in `index.html` (Leaflet + OpenStreetMap for the map, YouTube embeds for the streams).
- The streams are YouTube live broadcasts by Portal Netmadeira and Madeira-Web. When an operator restarts a stream it gets a new YouTube id: update `youtube:` in the `CAMS` list at the bottom of `index.html` (the operator's page, `page:`, shows the current one).
- Santa Cruz only has a snapshot camera; its pin links to it and offers the nearby Madeira Airport live stream.
- Local preview: `python3 -m http.server 8765` and open http://localhost:8765/ (YouTube does not play from a `file://` page).
