# Rochdale MVP — Data & Provenance Register v0.1

## Purpose

Record every source used in the prototype, its licence/access status, spatial/temporal characteristics, intended use and validation requirements.

## Source register

| Source | Intended use | Access | Licence / constraint | MVP status |
|---|---|---|---|---|
| Canal & River Trust Open Data / OGC API | canal network, assets and contextual waterway layers | API/catalogue | Verify dataset-specific terms before redistribution | Required |
| Environment Agency LiDAR DTM | terrain / embankment and drainage screening | Download/API services | Open Government Licence; attribution required | Required |
| Environment Agency LiDAR DSM | surface/building/vegetation context | Download/API services | Open Government Licence; attribution required | Useful |
| EA LiDAR time-stamped products | change analysis where repeat coverage exists | Download | OGL; survey dates vary | Required for change tests |
| CRT public notices / works pages | known works, stoppages, water constraints | Web | Public information; cite source; do not imply ownership of underlying database | Required |
| Weather/rainfall open data | rainfall and climate context | Public/open APIs where terms permit | Verify API terms | Required |
| Planning data | development pressure / potential value | Public authority portals | Terms vary; preserve source/provenance | Useful |
| Open environmental/flood datasets | hazard/context | Public/open | Verify source licence | Useful |
| Satellite imagery | potential change detection | Public/commercial | Sentinel open data where appropriate; commercial data only with approval | Experimental |

## Provenance rules

Every displayed claim must retain:

- source name
- source URL or dataset identifier
- access date
- relevant survey/data date
- transformation/processing applied
- licence/attribution requirement
- confidence level

## Licensing gate

No third-party dataset may be redistributed in a customer-facing product until its licence permits the intended use. Derived analytics should retain sufficient provenance to reproduce the result.

## Technical caution

Environment Agency LiDAR products report +/-15 cm RMSE vertical accuracy, but this does **not** mean that a difference of 15 cm between surfaces is automatically a real structural movement signal. Survey dates, transformations, vegetation, point density, processing and local conditions must be considered.

## Data quality labels

- **A — direct authoritative source**
- **B — authoritative contextual source**
- **C — open third-party contextual source**
- **D — inferred/derived signal**
- **E — unverified hypothesis**

The MVP must never present D or E as established condition facts.
