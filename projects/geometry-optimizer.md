# Geometry Optimizer (Strength-to-Weight Ranking)

This project is a geometry optimization / ranking tool I built to compare structural “girder-like” geometries and identify options with strong **strength-to-weight** performance.

The goal wasn’t a perfect industrial optimizer — it was to build a practical engineering workflow:
- define a performance metric
- generate candidate geometries
- evaluate them consistently
- rank and compare results
- validate with sanity checks (hand calcs / simple FEA comparisons)

> Note: Some code for this project was developed across different machines/versions and I’m rebuilding a clean, publishable repo structure. This page documents what I did and how the system worked.

---

## What it does (high level)
- Generates (or accepts) a set of candidate girder geometries (parameterized shapes)
- Computes a comparative score for each geometry, targeting:
  - high stiffness/strength proxy
  - low mass / material usage
- Produces a ranked list of candidates and a shortlist for deeper validation

---

## Inputs
Typical inputs (varies by run):
- span / length (L)
- loading assumptions (point load, distributed, etc.)
- boundary conditions (supported, fixed, etc.)
- geometry parameters (web thickness, flange width, height, cell count, etc.)
- material assumptions (density, E, yield proxy)

---

## Outputs
- Ranked candidate list (best → worst)
- Score breakdown per candidate (so it’s not a black box)
- A shortlist of top candidates for:
  - hand-check sanity verification
  - simple FEA comparison (where available)

---

## Why it’s useful
If you’re designing a structure (bridge, frame, airframe element, fixture), there are often many possible geometry families. A ranking tool helps you:
- explore the design space quickly
- justify why a chosen geometry is reasonable
- reduce time spent iterating blindly in CAD

---

## Validation / sanity checks
I used basic checks such as:
- comparing relative results to expected trends (e.g., deeper section → higher bending stiffness)
- spot-checking a few cases using hand calculations
- comparing a subset using simple FEA / simulation when feasible

---

## What I’m adding next
- Reconstructed code + parameter definitions
- Example runs with plots/tables
- A “case study” example:
  - requirements → candidate set → ranking → chosen geometry → verification

---

## Links
- Main portfolio: https://github.com/tuohyrhys/rhystuohy
- (Repo link will be inserted here when code is collected and organized)
