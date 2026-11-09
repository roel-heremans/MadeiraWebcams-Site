# Madeira Webcams

One page with a map of Madeira and live webcams for Porto Moniz, Paul do Mar, Jardim do Mar, Fajã da Areia, Calheta, Ponta do Sol, Ribeira Brava, Cabo Girão, Câmara de Lobos, Praia Formosa, Funchal Pontinha, Reis Magos, Santa Cruz, Machico and Porto Santo. Click a pin or a name to play the stream.

Live: https://roel-heremans.github.io/MadeiraWebcams-Site/

- Everything is in `index.html` (Leaflet + OpenStreetMap for the map, YouTube embeds for the streams).
- The streams are YouTube live broadcasts by Portal Netmadeira and Madeira-Web. When an operator restarts a stream it gets a new YouTube id: update `youtube:` in the `CAMS` list at the bottom of `index.html` (the operator's page, `page:`, shows the current one).
- Not every place has an embeddable stream: Jardim do Mar and Fajã da Areia are MEO Beachcam cameras (their site does not allow embedding, so the pins link out; Fajã da Areia also offers the Seixal stream). Cabo Girão has no camera of its own; its pin offers the Cruz da Caldeira stream. Santa Cruz only has a snapshot camera, plus the nearby Madeira Airport stream.
- Local preview: `python3 -m http.server 8765` and open http://localhost:8765/ (YouTube does not play from a `file://` page).
