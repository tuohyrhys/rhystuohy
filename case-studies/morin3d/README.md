# Morin 3D (Island Additive Manufacturing) | Design Engineering

**Disclosure:** I am currently in the process of obtaining permission to publicly share additional Morin 3D work product.  
Due to confidentiality obligations, I may not be able to share work product or client specific artifacts outside the organization.  
If you would like to discuss the details of my role further, feel free to contact me!

Last updated: 2026-01-22.

## Outcome Summary
- Shipped design to release artifacts for additive manufactured client hardware, including CAD, drawings, assemblies, BOMs, and release notes.
- Designed tolerance driven interfaces for calibrated industrial grade printing systems, with critical features typically specified within **±0.05 to 0.25 mm**.
- Completed an FEA informed redesign on a load bearing part and achieved **16% material reduction** while improving stiffness and durability.
- Built internal process tooling to improve traceability and standardize quoting and review.

---

## Context + Objective
Morin 3D produces functional additive manufactured components for real customers using calibrated industrial printing systems. The work requires clear interfaces, manufacturable geometry, and documentation that reduces ambiguity during manufacturing and assembly.

**Objective:** convert ambiguous requests into decision ready CAD and release artifacts that support quoting, manufacturing, assembly, and iteration with minimal back and forth.

---

## Tools + Artifacts
**Tools**
- Onshape (parametric CAD, assemblies, drawings)
- FEA tool (used for load bearing redesign, details redacted as needed)
- Internal templates (release checklist, revision notes, change summaries)
- Internal process tooling (print and process database, cost and time estimator)

**Artifacts in this folder**
- `brief.pdf` (one page project brief)
- `assets/` (figure placeholders now, annotated evidence images later)
- Optional: `drawings/` (redacted PDFs)
- Optional: `release-notes/` (revision log and decision notes, redacted)
- Optional: `process-tooling/` (screenshots of templates and estimators, sensitive values removed)

---

## Approach
- Translated requests into measurable requirements, including interfaces, serviceability, manufacturability, and schedule constraints.
- Reverse engineered existing parts into parametric CAD from scans and drawings.
- Designed large format additive geometry for process reality, including minimum thickness, overhang control, print orientation constraints, and post processing allowances.
- Defined interfaces with functional tolerances appropriate for calibrated industrial systems.
- Produced drawings, assemblies, and BOMs that reduce interpretation drift during manufacturing and assembly.
- Documented revisions using short change summaries so stakeholders can review quickly across concurrent jobs.
- Built internal process tooling that improves quoting consistency and traceability.

---

## Key Decisions
- Chose tolerance strategies that match function and process capability, rather than applying tight tolerances everywhere.
  - Evidence: Figure 3
- Defined interface references early to control alignment, clearance, and serviceability.
  - Evidence: Figure 2
- Designed geometry around additive constraints, including orientation, minimum thickness, and support avoidance on critical surfaces.
  - Evidence: Figure 5
- Used an FEA informed redesign approach for a load bearing part to remove low value material while maintaining or improving performance.
  - Evidence: Figure 4
- Standardized review and release artifacts to reduce iteration churn across multiple jobs.
  - Evidence: Figures 1, 6, 8
- Built internal process tooling to improve traceability and quoting consistency.
  - Evidence: Figure 7

---

## Results
- Produced integration ready release artifacts, including drawings, assemblies, BOMs, tolerance notes, revision notes, and mini design reports as needed.
- Interfaces typically designed within **±0.05 to 0.25 mm** for calibrated industrial printing systems, with tolerances applied to function critical features.
- Achieved **16% material reduction** on a load bearing redesign while improving stiffness and durability.
- Delivered internal process tooling, including a print and process database and a cost and time estimator, to standardize review and quoting workflows.

---

## Evidence Gallery
Figures are listed now so reviewers can see the evidence plan. Files will be added under `assets/` after permission to publish is confirmed.

**Figure 1: Release package overview**  
What it is: drawing excerpt, assembly view, BOM snippet, and revision note snapshot.  
What to notice: complete design to release bundle and traceability.  
Why it matters: proves release discipline, not just CAD.  
File: `assets/Figure_01_release-package.png` (pending)

**Figure 2: Interface map**  
What it is: annotated assembly view identifying the surfaces and features that control alignment and clearance.  
What to notice: which interfaces drive tolerances and failure risk.  
Why it matters: shows you engineer interfaces and integration.  
File: `assets/Figure_02_interface-map.png` (pending)

**Figure 3: Tolerance and fit notes excerpt**  
What it is: redacted drawing crop showing functional tolerance callouts and assembly notes.  
What to notice: where tolerances tighten and where they relax.  
Why it matters: links process capability to reliable integration.  
File: `assets/Figure_03_tolerance-notes.png` (pending)

**Figure 4: FEA informed redesign, before vs after**  
What it is: geometry comparison plus an excerpt of the analysis output.  
What to notice: material removed from low value regions, high torque regions, and retained where load flows.  
Why it matters: supports the 16% reduction claim with bounded evidence.  
File: `assets/Figure_04_fea-redesign.png` (pending)

**Figure 5: DFAM constraints and orientation decision**  
What it is: print orientation and risk zone markup for a representative part.  
What to notice: how geometry changes reduce supports, warp risk, and failure risk.  
Why it matters: shows manufacturability driven design decisions.  
File: `assets/Figure_05_orientation-constraints.png` (pending)

**Figure 6: Revision change summary excerpt**  
What it is: short change note listing what changed, why, and the impact.  
What to notice: scope control and decision clarity.  
Why it matters: reduces review time and iteration churn.  
File: `assets/Figure_06_change-summary.png` (pending)

**Figure 7: Internal process tooling excerpt**  
What it is: redacted screenshot of a template, database, or estimator used to standardize quoting and review.  
What to notice: consistent fields and traceability structure.  
Why it matters: shows impact beyond a single part.  
File: `assets/Figure_07_process-tooling.png` (pending)

**Figure 8: Release checklist or review rubric**  
What it is: checklist that gates release quality before sending artifacts out.  
What to notice: verification minded structure.  
Why it matters: shows reliable process and repeatability.  
File: `assets/Figure_08_release-checklist.png` (pending)

---

## GitHub Links
- Brief: `brief.pdf`
- Evidence images: `assets/`
- Optional drawings: `drawings/`
- Optional revision notes: `release-notes/`
- Optional process tooling: `process-tooling/`

---

## Next Iteration
- Add an interface control sheet for the top three mating interfaces, including datum scheme and acceptance criteria.
- Add a lightweight tolerance stack table for one critical interface to make integration risk visible during review.
- Expand estimator inputs to include support time, post processing steps, and tolerance criticality, then track its effect on quoting consistency.

---

## Contact
If you would like to discuss the details of my role further, please contact me:
- Email: rhys.tuohy@mail.utoronto.ca
- LinkedIn: https://www.linkedin.com/in/rhys-tuohy

---

## Credits
Role: Design Engineering Intern to Contract  
Organization: Morin 3D, Island Additive Manufacturing  
Dates: Jul 2025 to Present
