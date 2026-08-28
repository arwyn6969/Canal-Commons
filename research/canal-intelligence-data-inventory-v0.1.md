# Canal Intelligence — Data Inventory v0.1

## Objective

Identify the minimum legally usable data stack needed to create a useful decision-support demonstrator without depending on confidential CRT systems.

## Tier 1 — Core spatial/infrastructure data

| Data | Likely source | MVP use | Confidence |
|---|---|---|---|
| Canal centreline / waterway geography | CRT open data / ArcGIS | Corridor geometry | High |
| Locks, bridges, aqueducts, culverts and other structures where published | CRT/open geospatial sources | Asset inventory | Medium–High |
| Towpaths/access | CRT/open geospatial sources | Access and consequence analysis | High |
| Administrative boundaries | ONS/Open Government data | Customer/reporting geography | High |
| Buildings/land use | Ordnance Survey/open datasets where licensed | Exposure and development context | High |
| Roads/rail/critical infrastructure | OpenStreetMap / government open data, licence checked | Consequence of failure / logistics | High |

## Tier 2 — Hazard and environmental data

| Data | Source family | MVP use | Confidence |
|---|---|---|---|
| Rainfall/weather | Met Office / Environment Agency / open datasets | Event and stress indicators | High |
| Flood risk | Environment Agency | External hazard context | High |
| Terrain/elevation | Environment Agency / national LiDAR where available | Embankment/low-point context | High |
| Geology/soils | BGS / government data | Potential piping/ground-risk context | High |
| Land cover/vegetation | Sentinel/Copernicus / open imagery | Change detection | High |
| Surface-water context | Environment Agency / open data | Water interaction | Medium–High |

## Tier 3 — Remote sensing

### Sentinel-1 SAR / InSAR

Potential use: detect persistent ground-surface movement around embankments, retaining structures and adjacent land.

Important limitation: InSAR does not directly diagnose a canal leak or prove structural failure. It is a screening signal requiring engineering validation.

### Sentinel-2 optical imagery

Potential use: vegetation/water/land-cover change and post-event comparison.

### Commercial satellite/drone imagery

Potential future premium layer, not required for MVP.

## Tier 4 — Event and operational information

- CRT incident and stoppage notices
- published breach/failure case studies
- CRT winter works / maintenance updates
- navigation restrictions
- water-management restrictions
- planning applications
- local authority infrastructure plans
- public procurement notices
- environmental permits

These are potentially more commercially useful than raw imagery because they connect risk to actual decisions and spending.

## Tier 5 — Commercial enrichment

Potential future layers:

- property/development pipeline
- canalside land ownership where lawfully available
- heat-demand / building-energy information
- freight origins/destinations
- local business density
- tourism/footfall proxies
- construction logistics
- insurance/risk indicators where obtainable

These should be added only where there is a clear paying use case.

## Data governance rules

1. Record source, licence, access date and transformation for every dataset.
2. Do not scrape or ingest confidential/proprietary CRT data without permission.
3. Do not imply that public data represents CRT's complete asset register.
4. Preserve provenance so every risk signal can be traced back to its source.
5. Separate observation from inference.
6. Treat any engineering-risk output as screening/prioritisation, not a safety determination.

## Minimum viable stack

The first demonstrator should work with:

**canal/asset geography + terrain + geology/soil + rainfall/flood context + satellite change indicators + published incidents/works + development/exposure context.**

If the model cannot produce a useful result from that stack, adding expensive sensors is premature.

## Commercial implication

The data itself should not be the product. The product is the **decision layer** that converts disparate data into a ranked list of inspection, investment, resilience or development opportunities with evidence and confidence attached.
