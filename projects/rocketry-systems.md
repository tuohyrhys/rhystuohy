# Rocketry Systems (Design, Simulation, Controls, Test)

Flight vehicles, instrumentation, and simulation-driven GNC work executed with an engineering loop: **define → build → test → iterate**.

---

## At a glance
| Area | Summary | Tools / Artifacts |
|---|---|---|
| Flight vehicles | Rockets across A–E motors, including ~2 m vehicle | CAD, build photos, flight log |
| Instrumentation | Onboard sensing + time-series logging; calibration and sampling constraints | logs, preprocessing notes, plots |
| GNC concepts | Waypoint-style guidance under actuator/timing limits; simulation → prototype workflow | Simulink sweeps, bench validation |
| Test approach | Acceptance criteria + configuration logging + incremental risk | checklist, test matrix |

---

## Key results / benchmarks
- Built and flown multiple vehicles (A–E range), including a **~2 m** airframe.
- Ran a **10-flight** program on smaller vehicles to validate build/integration/recovery choices before scaling.
- Targeted high-rate logging in some tests (e.g., **~1 ms** sampling goal) and documented practical limits (timing, storage, noise).
- Waypoint guidance benchmark (simulation): **~5.7 m** mean closest-approach error across **10** randomized targets (50–200 m XYZ).

---

## System breakdown

## 1) Flight vehicles (design + build)
**Scope**
- Airframe configuration, stability considerations, recovery integration, manufacturing constraints, and iteration.

**Work performed**
- Designed and built rockets across multiple sizes and motor classes; iterated designs based on build outcomes and flight behavior.
- Standardized integration details where possible (interfaces, fasteners, access, recovery packing).

**Artifacts**
- Build photos: `../assets/img/rocketry/`
- Flight log (table): `../assets/files/rocketry/flight-log.csv` (or PDF)

---

## 2) Instrumentation + data logging (flight-ish / test)
**Scope**
- Sensor integration + logging workflow; time-series handling (sampling, calibration, noise, synchronization).

**Work performed**
- Integrated microcontroller-based logging and structured time-series outputs to support analysis.
- Focused on signal quality: sampling constraints, noise sources, calibration drift, and event detection.

**Artifacts**
- Example raw log + cleaned dataset: `../assets/files/rocketry/`
- Plot(s): `../assets/img/rocketry/`

---

## 3) Guidance / control concepts (simulation-driven)
**Scope**
- Simulation-to-implementation exploration for trajectory guidance under constraints (actuator limits, loop timing, stability tradeoffs).

**Work performed**
- Built Simulink assets for parameter sweeps and tuning studies (feed-forward concepts + basic PID prototypes).
- Investigated fin-actuation guidance concepts and waypoint-style tracking under constraints.

**Artifacts**
- Simulink overview screenshot: `../assets/img/rocketry/simulink-overview.png`
- Parameter sweep plot(s): `../assets/img/rocketry/`
- Tracking metric plot(s): `../assets/img/rocketry/closest-approach.png`

---

## 4) Test approach (verification mindset)
- Define acceptance criteria before testing (what “success” means).
- Log configuration + environment assumptions (mass, motor, weather, firmware version, sensor rates).
- Start small, validate subsystems, then scale risk.
- Record failures and the design changes they trigger.

---

## Evidence (drop-in visuals)
> Replace filenames below with your actual uploads.

![Vehicle build / assembly](../assets/img/rocketry/vehicle-assembly.jpg)

![Bench setup / instrumentation](../assets/img/rocketry/bench-setup.jpg)

![Simulink model overview](../assets/img/rocketry/simulink-overview.png)

![Closest-approach metric plot](../assets/img/rocketry/closest-approach.png)

---

## Links
- Main portfolio: https://github.com/tuohyrhys/rhystuohy
