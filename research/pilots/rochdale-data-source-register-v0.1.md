# Rochdale Pilot — Data Source Register v0.1

**Date:** 2026-08-28

| Source | Intended use | Access route | Licence/provenance check | Status |
|---|---|---|---|---|
| CRT Open Data | canal/network/assets and catalogue discovery | CRT ArcGIS OGC API | Required before redistribution | Identified |
| CRT public notices | live works, stoppages, operational context | CRT website / public notices | Public-source citation | Identified |
| Environment Agency | flood-risk / hydrology context | data.gov.uk / EA datasets | Required per dataset | Identified |
| BGS | geology/ground context | BGS public datasets where available | Required per dataset | Identified |
| Copernicus Sentinel | remote observation / change signals | Copernicus Data Space | Check product licence and processing requirements | Identified |
| UK government planning/open data | development and land-use opportunity context | planning/data.gov.uk/local sources | Required per dataset | Identified |
| Local authority GIS | public realm, planning, transport context | Manchester / Rochdale public datasets | Required per dataset | Identified |
| Weather/rainfall datasets | drought/rainfall/change context | Met Office / EA / other permitted public sources | Required per dataset | Identified |
| Public stoppage aggregators | discovery/cross-check only | public web | Use as secondary evidence, not authoritative source | Identified |

## Data governance rule

No dataset enters a customer-facing product until:
1. provenance is recorded;
2. licence/terms are checked;
3. update frequency is recorded;
4. limitations are documented;
5. derived-data rights are understood.

## Current authoritative source preference

1. Navigation authority / government primary source.
2. Public statutory/open dataset.
3. Reputable research source.
4. Secondary aggregator only for discovery or cross-checking.

## Immediate data work

- Query CRT OGC API catalogue and identify collections relevant to Rochdale.
- Define a stable corridor geometry.
- Acquire permitted terrain/geology/flood/rainfall/satellite layers.
- Create a source metadata table with acquisition date and licence.
- Avoid scraping or redistributing restricted datasets without permission.
