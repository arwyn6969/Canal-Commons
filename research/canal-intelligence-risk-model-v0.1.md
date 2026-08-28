# Canal Intelligence — Risk Model v0.1

## Purpose

Create a transparent screening model for prioritising where additional investigation may be valuable. This is **not an engineering safety model** and must never be presented as one.

## Unit of analysis

A practical MVP should divide the pilot corridor into consistent analytical segments (for example 100–250 m) and separately score discrete structures such as locks, culverts and bridges where sufficient data exists.

## Proposed score

`Priority = Consequence × Hazard × Evidence Gap × Change Signal`

Each component is normalised 0–10.

### 1. Consequence (0–10)

Measures what happens if the asset/segment fails.

Possible inputs:
- people/public exposure
- navigation disruption
- nearby homes/businesses
- roads/rail/utilities
- environmental consequence
- heritage significance
- estimated repair/access complexity

### 2. Hazard (0–10)

Measures external/structural factors associated with failure modes.

Possible inputs:
- embankment geometry
- slope/elevation context
- geology/soil susceptibility
- flood/water pressure context
- historical incidents
- known leakage/defect reports
- asset age/type where available
- climate exposure

### 3. Evidence Gap (0–10)

Measures how poorly the risk is currently observed by the public data stack.

High score means **we know less**, not that the asset is more dangerous.

This is important because the commercial product may be valuable precisely where existing information is incomplete.

### 4. Change Signal (0–10)

Measures whether recent external observations show unusual change.

Possible inputs:
- InSAR deformation trend
- vegetation change
- surface-water change
- unusual rainfall/water events
- repeated incident reports
- construction/land-use change

## Output categories

- **Priority A:** independent technical review/data acquisition potentially justified
- **Priority B:** monitor and seek additional evidence
- **Priority C:** no immediate additional signal from MVP data

No category should be labelled “safe” or “unsafe”.

## Llangollen lesson

The December 2025 Llangollen breach is a key design test. CRT's interim investigation says a long-term, deep-seated leak beneath the canal bed was not visible through the existing inspection regime and may have produced internal erosion/piping before collapse. This demonstrates why the model should include **subsurface-risk proxies and evidence gaps**, while also demonstrating why remote sensing cannot be treated as proof of a hidden defect.

Source: https://canalrivertrust.org.uk/news-and-views/news/weve-published-our-initial-findings-on-the-llangollen-canal-breach

## Example scoring logic

A segment might receive:

- Consequence 8
- Hazard 6
- Evidence gap 8
- Change signal 5

The product should not simply multiply these numbers and call the result “risk”. Instead, it should show the four components separately and explain why the segment was prioritised.

## Validation requirement

The model must eventually be back-tested against known historical incidents and reviewed by qualified infrastructure/engineering professionals.

Success is not “the algorithm predicts every failure”. A realistic MVP target is:

> **Can the model produce a more useful and explainable shortlist for where additional inspection or data collection should be considered?**

## Commercial output

The valuable deliverable is a ranked decision pack containing:

1. corridor map
2. top-priority segments/assets
3. evidence behind each ranking
4. uncertainty/confidence
5. recommended next data acquisition
6. indicative consequence/cost bands where defensible
7. suggested engineering questions for a qualified professional

This turns data into a product that can potentially be sold to infrastructure owners, engineering firms, insurers, developers or public authorities.
