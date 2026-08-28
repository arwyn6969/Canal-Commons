# Rochdale Canal Intelligence MVP v0.1

**Status:** Build specification / evidence-led prototype
**Branch:** `research/rochdale-mvp-v0.1`
**Date:** 2026-08-28

## Objective

Test whether Canal Commons can create a commercially useful decision layer by combining existing public/open waterway, terrain, environmental and contextual datasets into a prioritised map of risks and opportunities.

This is **not** an engineering safety assessment, condition survey, or replacement for Canal & River Trust asset-management systems.

## Pilot area

Rochdale Canal corridor, Manchester to the summit/Tuel Lane area, with an initial analytical window of approximately 20 km. The corridor is intentionally selected because it combines urban infrastructure, locks, water-management constraints, active works, development pressure and environmental/climate questions.

## Current evidence anchors

- CRT publishes an OGC API for its open-data catalogue, allowing programmatic discovery of datasets. See `https://data-canalrivertrust.opendata.arcgis.com/api/search/definition/`.
- CRT's current boating guidance records significant water scarcity on the Rochdale and operational windows for Locks 1–13.
- CRT's current five-year works plan includes future Rochdale lock-gate work, demonstrating an active maintenance pipeline.
- Environment Agency LiDAR is available under the Open Government Licence; time-stamped products include 25 cm, 50 cm, 1 m and 2 m resolutions and report vertical accuracy of +/-15 cm RMSE.

## MVP questions

1. Can we legally and reproducibly assemble useful cross-source data for the corridor?
2. Can the data reveal a prioritisation signal not obvious from a single source?
3. Can we express the result as a decision a professional could act upon?
4. Can an engineering, infrastructure, public-sector, developer or related customer identify a real use case?
5. Will at least one credible organisation pay for a pilot or equivalent professional engagement?

## Initial data layers

### Core
- CRT canal/asset/open datasets
- Environment Agency LiDAR DTM/DSM and survey metadata
- OS/open geographic context where licensing permits
- flood/environment datasets
- rainfall/weather and drought indicators
- publicly documented CRT notices, stoppages and works

### Contextual
- planning applications and development activity
- land use / brownfield / regeneration context
- transport and access constraints
- publicly documented incidents and community observations
- environmental opportunity indicators

### Future / optional
- Sentinel-1/2 satellite data and derived change indicators
- commercial satellite data only if a customer use case justifies cost
- specialist geophysics only as a later validation layer

## Risk/opportunity model v0.1

Each candidate location/asset receives separate scores rather than a single opaque AI score:

- **Hazard signal (0–5):** evidence of physical/environmental pressure
- **Consequence (0–5):** plausible operational/economic/community consequence
- **Change signal (0–5):** evidence that conditions may be changing
- **Evidence gap (0–3):** uncertainty that may justify inspection or investigation
- **Opportunity signal (0–5):** potential commercial, resilience or environmental opportunity

The prototype should show the component scores, source evidence and confidence. No automated output should claim an asset is unsafe.

## First deliverable

A professional PDF/HTML-style decision brief containing:

1. corridor overview map
2. data/provenance register
3. ranked top 10 investigation/opportunity locations
4. evidence cards for each location
5. confidence and limitations
6. suggested next investigation/action
7. estimated commercial decision value where defensible
8. explicit distinction between known fact, inference and hypothesis

## Commercial hypothesis

The product is not "monitoring as a replacement for CRT". It is a cross-data intelligence layer that may help third parties answer:

> Where should we investigate, spend, develop, insure, finance or intervene next, and what evidence supports that decision?

Potential buyers/users:
- engineering and inspection firms
- local authorities
- infrastructure owners
- developers
- energy developers
- insurers/risk specialists
- investors/project financiers
- CRT and other waterway organisations

## Commercial validation

Target outcome after the demonstrator:

- 8+ structured discovery conversations
- 3+ independently expressed unmet needs
- 1+ credible paid-pilot or paid-analysis opportunity

A suggested pilot price of £5k–£25k is a **test range only**, not a market assumption.

## Kill criteria

Stop or materially redesign if:

- data cannot be obtained/licensed reproducibly;
- the output merely duplicates existing customer capability;
- domain professionals cannot identify a decision it would change;
- no plausible budget owner exists;
- customers value the concept but will not pay for it;
- the signal cannot be validated sufficiently for professional use;
- legal/liability exposure is disproportionate to commercial value.

## Success criteria

The MVP succeeds if it produces at least one decision-relevant insight that:

1. is supported by multiple independent sources;
2. was not obvious from a single dataset;
3. can be explained to a professional without exaggerated claims;
4. suggests a concrete next action;
5. has a plausible economic value to a named customer.

## Build discipline

Do not build a production platform, install a sensor network, buy boats, launch a token, or raise external capital on the strength of this MVP. The demonstrator exists to buy information cheaply and determine whether a real commercial product exists.
