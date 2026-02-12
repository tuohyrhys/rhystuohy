# Embedded Rocket GNC | Simulation to Hardware

Status: content complete. Figures are listed with placeholders while visuals are being added. Last updated: 2026-01-22.

## Outcome Summary
- Built a simulation to hardware workflow for a rocket guidance, navigation, and control concept under actuator and power constraints.
- Developed a waypoint guidance harness with randomized variation to test robustness across scenarios.
- Defined explicit scoring metrics and kept traceable tuning notes so iteration is reviewable.
- Implemented a feed forward fin deflection approach based on pre set simulations, not state estimation.

Optional metric, include only if you are comfortable and it is accurate:
- Achieved **5.7 m** mean closest approach error across **10** randomized targets at **50 to 200 m**.

---

## Context + Objective
GNC work is easy to make look impressive and easy to make non reproducible. The goal here was to build a workflow that is clear, testable, and transferable from simulation to a constrained embedded system.

**Objective:** create a decision ready GNC pipeline that defines success metrics, tests robustness, and produces artifacts that guide embedded implementation.

---

## Tools + Artifacts
**Tools**
- MATLAB and Simulink (modeling and simulation)
- Embedded microcontroller code (ESP32 or Arduino, C or C++)
- Python (analysis and plotting as needed)
- Test harness scripts and parameter sets

**Artifacts in this folder**
- `brief.pdf` (one page project brief)
- `assets/` (figure placeholders now, annotated evidence images later)
- Optional: `models/` (Simulink screenshots, parameter sets)
- Optional: `code/` (embedded code, helpers, scripts)
- Optional: `notes/` (scoring metric definition, tuning log)

---

## Approach
- Defined the guidance objective and a scoring metric that can be computed in simulation and compared across scenarios.
- Built a waypoint harness and randomized key environmental and system variables to probe robustness.
- Generated fin deflection schedules from pre set simulations and implemented a feed forward control approach for the embedded target.
- Logged each iteration with what changed, why, and its effect on the metric.
- Planned a hardware validation path that matches the simulation outputs to measurable signals.

---

## Key Decisions
- Used explicit scoring metrics instead of qualitative flight descriptions.
  - Evidence: Figure 2
- Tested robustness using randomized scenario variation rather than a single nominal case.
  - Evidence: Figure 3
- Chose a feed forward fin deflection schedule approach based on pre set simulations given project constraints.
  - Evidence: Figure 4
- Designed the pipeline so the same parameter sets drive both simulation runs and embedded outputs.
  - Evidence: Figure 5

---

## Results
- Created a repeatable simulation harness that evaluates guidance performance across varied scenarios.
- Produced fin deflection schedules and a transfer path for implementing them on constrained hardware.
- Delivered a traceable tuning log that links iteration decisions to metric changes.
- Established a hardware validation plan with measurable acceptance targets.
- Mean closest approach error: **5.7 m** across **10** randomized targets at **50 to 200 m**.

---

## Evidence Gallery
Figures are listed now so reviewers can see the evidence plan. Files will be added under `assets/`.

**Figure 1: System overview**  
What it is: architecture diagram from simulation harness to embedded implementation.  
What to notice: where metrics are computed and where schedules are generated.  
Why it matters: shows an end to end workflow rather than a single model.  
File: `assets/Figure_01_system-overview.png` (coming)

**Figure 2: Scoring metric definition**  
What it is: definition of the success metric and how it is computed.  
What to notice: clear units and conditions.  
Why it matters: enables objective comparison across iterations.  
File: `assets/Figure_02_scoring-metric.png` (coming)

**Figure 3: Robustness harness**  
What it is: list or diagram of randomized variables and scenario generation logic.  
What to notice: ranges and distribution assumptions.  
Why it matters: tests performance beyond nominal conditions.  
File: `assets/Figure_03_robustness-harness.png` (coming)

**Figure 4: Feed forward fin deflection schedules**  
What it is: example fin deflection schedules derived from simulations.  
What to notice: how schedules change with target and conditions.  
Why it matters: connects simulation outputs to implementable control signals.  
File: `assets/Figure_04_fin-schedules.png` (coming)

**Figure 5: Simulation to hardware mapping**  
What it is: table mapping simulation parameters and outputs to embedded variables and units.  
What to notice: unit consistency and parameter ownership.  
Why it matters: reduces implementation errors and speeds integration.  
File: `assets/Figure_05_sim-hw-mapping.png` (coming)

**Figure 6: Tuning log excerpt**  
What it is: change log showing what changed, why, and the effect on the metric.  
What to notice: iteration discipline and traceability.  
Why it matters: proves engineering process under uncertainty.  
File: `assets/Figure_06_tuning-log.png` (coming)

**Figure 7: Validation plan**  
What it is: staged test plan from bench tests to flight tests with acceptance checks.  
What to notice: measurable targets and what signals are recorded.  
Why it matters: shows verification mindset and practical execution.  
File: `assets/Figure_07_validation-plan.png` (coming)

---

## GitHub Links
- Brief: `brief.pdf`
- Evidence images: `assets/`
- Optional models: `models/`
- Optional code: `code/`
- Optional notes: `notes/`

---

## Next Iteration
- Add a standardized scenario suite and export plots for each run to support quick review.
- Record unit tests for schedule generation and parameter bounds checking.
- Validate schedule execution timing and actuator saturation limits on hardware.

---

## Contact
If you would like to discuss the workflow, scoring metrics, or hardware constraints in more detail, please contact me:
- Email: rhys.tuohy@mail.utoronto.ca
- LinkedIn: https://www.linkedin.com/in/rhys-tuohy

---

## Credits
Role: Guidance, Navigation, and Control  
Dates: 2024 to Present
