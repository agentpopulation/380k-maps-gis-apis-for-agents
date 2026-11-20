## Maps and GIS API endpoints, snapshot 15 Nov 2026

- 387,310 endpoints passed a keyless data call, tested 10–15 Nov 2026 (IST)
- 18,772 services · 247 country codes · 247,162 keyless JSON rows

### Download

- `Maps_GIS_API_Endpoints_AgentPopulation_Snapshot_2026-11-15.csv.gz`: the full list, 387,310 rows, 14.9 MB gzipped (126.9 MB as CSV), SHA-256 `d652abd514ced1278ddc88aaf6ed328566bb6ff49572c311b4e11a97807ac5b9`
- `SHA256SUMS.txt`: the checksum of that file

Check the download in the folder that holds both files:

```bash
sha256sum -c SHA256SUMS.txt          # Linux
shasum -a 256 -c SHA256SUMS.txt      # macOS
certutil -hashfile Maps_GIS_API_Endpoints_AgentPopulation_Snapshot_2026-11-15.csv.gz SHA256   # Windows: compare with SHA256SUMS.txt
```

Then `gunzip Maps_GIS_API_Endpoints_AgentPopulation_Snapshot_2026-11-15.csv.gz` and pass the CSV path to the examples or to `node tools/test-endpoints.mjs`. The repository itself holds a 1,000-row sample and the services list.

### What's in it for you

- 🤖 Agent tools: 70,229 · Wrap one layer query as a get_place_layer tool: pass a point, bounding box or country code, return the matching features (boundary name, parcel id, zoning class or address) with a timeout.
- 📱 App features: 98,806 · Add base maps, orthophotos and vector layers to an app map: read the service layer list once, then request the map or features for the visible area.
- 🧠 Grounding and data pipelines: 69,099 · Load place names, postal codes, boundaries and land-use layers on a schedule into your own store, so an agent can turn a place name into coordinates and a region and cite a dated source.
- 🧪 Evals and testing: 387,310 · Run your map tool against a fixed set of URLs across formats; check that features, coordinates and layer lists parse, and keep last_tested as the baseline for your own re-tests.

### Changes

- First release
- Left out: 7 rows with an email-like address.
- Left out: 1,228 ArcGIS Survey123 layers (they can hold people's form answers).
- Left out: 1 camera or image URL (webcam and camera feeds, picture and video files).
- Left out: 2 class-exercise copies of the same few ArcGIS Online layers (Miami Beach sea level rise, high-risk areas without shelter, flooded areas, sea level rise and storm surge maps) across many organisations, many with a person's name in the title.
- Left out: 65 layers marked editable in the title (they can hold entries that people added).
- Left out: 107 ArcGIS layers that keep a form's default service name (they can hold people's form answers).
- Left out: 6 rows that passed a data call only from a network location in India.
- Left out: 2,708 ArcGIS class or coursework layers (lab, assignment, exam, quiz, lesson, exercise, tutorial and final-project layers, copies of class layers, layers named for a person or a person's home, and layers whose name ends in a person's name or holds a student number).
- Left out: 356 ArcGIS layers that hold reports, comments, submissions or form responses sent in by the public.
- Overlap: 1,913 of these URLs are also in 190k-weather-apis-for-agents.
- Overlap: 4,619 of these URLs are also in 270k-transit-apis-for-agents.
- Overlap: 3,014 of these URLs are also in 270k-water-apis-for-agents.
- Overlap: 1,194 of these URLs are also in 130k-finance-economy-apis-for-agents.
- Overlap: 6,260 of these URLs are also in 130k-india-apis-for-agents.
- Overlap: 1,729 of these URLs are also in 86k-oceans-apis-for-agents.
- Overlap: 560 of these URLs are also in 20k-air-quality-apis-for-agents.
- Overlap: 247,162 of these URLs are also in 2.5m-agent-ready-apis.
- Overlap: 26 of these URLs are also in 6.5k-wildfire-apis-for-agents.
- Overlap: 1,833 of these URLs are also in 24k-traffic-apis-for-agents.
- Overlap: 146 of these URLs are also in 12k-parking-apis-for-agents.
- Overlap: 83 of these URLs are also in 10k-earthquake-apis-for-agents.
- Overlap: 4 of these URLs are also in 5.2k-volcano-tsunami-apis-for-agents.

On the date in last_tested (IST), one GET to the URL, sent with no key, returned HTTP 2xx and a non-empty data body. HTML pages and empty results did not pass. The format column records what came back. This is a test result for that date, not a promise that the URL answers today. Licences, terms, rate limits, accuracy and freshness were not reviewed. Endpoints are URLs, not separate APIs; many share one service. This pack was tested 10–15 Nov 2026; snapshot 15 Nov 2026.

For the latest tested endpoints, search agentpopulation.com/apis. This pack is a snapshot from 15 Nov 2026.

Credit: Maps and GIS API endpoints by AgentPopulation (https://agentpopulation.com), CC BY 4.0, snapshot 15 Nov 2026.

Compiled by [AgentPopulation](https://agentpopulation.com) with [AP Desk](https://github.com/agentpopulation/apdesk) · corrections: [@agentpopulation](https://x.com/agentpopulation) on X
