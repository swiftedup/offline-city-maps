# Offline city maps

Street-level vector map files for 60 US cities: the 31 largest by population, plus the largest city in every other state, so all 50 states and DC are covered.

Each city is one [PMTiles](https://docs.protomaps.com/pmtiles/) file (vector tiles, zoom 0–14; Las Vegas goes to zoom 15). The files are attached to this repository's [releases](../../releases), not stored in the repository itself.

## Using the files

Download a city from the latest release:

```
https://github.com/swiftedup/offline-city-maps/releases/download/maps-v1/<city>.pmtiles
```

`SHA256SUMS.txt` in the same release lists a checksum for every file.

Any PMTiles-aware map library can read them, for example MapLibre Native or MapLibre GL JS. The tiles use the Protomaps basemap layer schema (version 4).

## Data source and license

The map data is © [OpenStreetMap](https://www.openstreetmap.org/copyright) contributors, available under the [Open Database License](https://opendatacommons.org/licenses/odbl/). The tiles were extracted from the [Protomaps](https://protomaps.com) daily basemap build of 2026-11-09.

If you use these files, you must credit OpenStreetMap.
