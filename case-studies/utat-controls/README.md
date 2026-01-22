# UTAT Rocketry | Systems and Controls Modeling

Status: content complete. Figures are listed with placeholders while visuals are being added. Last updated: 2026-01-22.

## Outcome Summary
- Produced integration focused schematics and block diagrams to clarify subsystem boundaries and signal flow.
- Extended a MATLAB and Simulink model to support variable thrust and propulsion profiles.
- Documented assumptions, sensitivity drivers, and validation priorities so the model can guide test planning and design decisions.
- Packaged artifacts so new contributors can understand interfaces and pick up work quickly.

---

## Context + Objective
The University of Toronto Aerospace Team Rocketry division develops rockets under tight mass, reliability, and integration constraints. Controls and propulsion modeling has to be usable by others, and it must make assumptions and limitations obvious.

**Objective:** create decision ready models and diagrams that reduce ambiguity across subteams and enable structured validation.

---

## Tools + Artifacts
**Tools**
- MATLAB and Simulink
- Systems diagrams and interface schematics (P and ID style where helpful)
- Versioned modeling notes (assumptions, parameters, and validation plan)

**Artifacts in this folder**
- `brief.pdf` (one page project brief)
- `assets/` (figure placeholders now, annotated evidence images later)
- Optional: `models/` (non sensitive model screenshots or redacted blocks)
- Optional: `notes/` (assumptions, parameter list, validation plan)

---

## Approach
- Mapped subsystem boundaries and interfaces before tuning or optimizing models.
- Built or extended Simulink blocks to represent variable thrust and propulsion dynamics.
- Wrote assumptions explicitly and separated constants, tuned parameters, and measured inputs.
- Identified sensitivity drivers that can change outcomes, then flagged them for validation.
- Defined model outputs that are directly useful for decision making, such as thrust profiles, trajectories, or stability margins depending on scope.
- Packaged the model and notes so another contributor can run it and reproduce results.

---

## Key Decisions
- Chose diagram first workflows to clarify interfaces before adding complexity to the model.
  - Evidence: Figure 1, Figure 2
- Structured the Simulink model so propulsion inputs can be swapped without rewriting the full system.
  - Evidence: Figure 3
- Documented uncertainty and sensitivity drivers so the model supports validation planning.
  - Evidence: Figure 4, Figure 5
- Defined a short validation plan that ties model outputs to measurable tests.
  - Evidence: Figure 6

---

## Results
- Produced interface and signal flow diagrams that reduce integration ambiguity across subteams.
- Extended a MATLAB and Simulink model to accept variable thrust profiles and propulsion inputs.
- Delivered an assumptions and sensitivity note so reviewers can evaluate model limits quickly.
- Created a validation priority list that turns open questions into testable steps.

---

## Evidence Gallery
Figures are listed now so reviewers can see the evidence plan. Files will be added under `assets/`.

**Figure 1: System block diagram**  
What it is: high level system diagram showing subsystems and signal flow.  
What to notice: interfaces and defined inputs and outputs.  
Why it matters: makes integration boundaries clear before implementation.  
File: `assets/Figure_01_system-block-diagram.png` (coming)

**Figure 2: Interface schematic**  
What it is: interface diagram that specifies what data moves between subsystems and at what rate.  
What to notice: clear ownership and dependencies.  
Why it matters: reduces integration errors and ambiguous handoffs.  
File: `assets/Figure_02_interface-schematic.png` (coming)

**Figure 3: Variable thrust modeling block**  
What it is: Simulink block or subsystem that accepts variable thrust profiles.  
What to notice: parameterization and how the profile is injected into dynamics.  
Why it matters: supports realistic propulsion behavior and scenario testing.  
File: `assets/Figure_03_variable-thrust-block.png` (coming)

**Figure 4: Assumptions and parameter table**  
What it is: table separating constants, tuned parameters, and measured inputs.  
What to notice: which parameters drive outcomes and which are placeholders.  
Why it matters: makes uncertainty explicit and reviewable.  
File: `assets/Figure_04_assumptions-parameters.png` (coming)

**Figure 5: Sensitivity drivers**  
What it is: short list or plot showing which parameters most affect the outputs.  
What to notice: ranked sensitivity and the conditions assumed.  
Why it matters: tells the team what to validate first.  
File: `assets/Figure_05_sensitivity-drivers.png` (coming)

**Figure 6: Validation plan**  
What it is: 5 to 10 bullet plan connecting model outputs to measurable tests.  
What to notice: clear next steps and acceptance criteria.  
Why it matters: turns the model into a decision tool, not a sandbox.  
File: `assets/Figure_06_validation-plan.png` (coming)

---

## GitHub Links
- Brief: `brief.pdf`
- Evidence images: `assets/`
- Optional model artifacts: `models/`
- Optional notes: `notes/`

---

## Next Iteration
- Add a simple test harness that runs a standard scenario set and exports key outputs for review.
- Tie each sensitivity driver to a measurement plan and a target accuracy range.
- Add model version tags and a change log so reviewers can track what changed and why.

---

## Contact
If you would like to discuss my contributions or modeling approach in more detail, please contact me:
- Email: rhys.tuohy@mail.utoronto.ca
- LinkedIn: https://www.linkedin.com/in/rhys-tuohy

---

## Credits
Role: Systems and Controls Modeling  
Organization: University of Toronto Aerospace Team, Rocketry  
Dates: [add your start date] to Present
