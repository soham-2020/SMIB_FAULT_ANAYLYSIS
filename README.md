Overview
Developed an advanced Simulink model of a Single Machine Infinite Bus (SMIB) system — representing a 60 MVA synchronous generator connected to a large power grid.
The model investigates transient instability during a three-phase fault on the transmission line, analyzing how system parameters affect synchronization and damping.

Objective

To analyze the transient stability of a synchronous generator during severe grid disturbances and identify methods to maintain synchronization using control mechanisms.
Technical Highlights
1. Synchronous Machine Modeling

Implemented the Simscape Electrical Synchronous Machine (Two-Axis dq Model).

Used per-unit (pu) system for machine parameters.

Extracted key outputs: rotor speed (ωₘ), torque (Tₑ), load angle (δ), and terminal voltage (Vₜ).

2. Governor & Turbine Control

Modeled mechanical input control (Pm) via feedback of speed deviation (Δω).

Stabilized system frequency by dynamically matching turbine input with electrical load demand.

3. Excitation Control System

Controlled field voltage (Vf) using reference voltage (Vref) and terminal feedback (Vt).

Regulated reactive power (Qₑₒ) and maintained system voltage stability.

4. Transient Stability Analysis

Simulated a three-phase fault and monitored:

Load Angle (δ)

Active Power (Pₑₒ)

Reactive Power (Qₑₒ)

Rotor Speed (ωₘ)

Time Period	System Behavior	Engineering Meaning
0–1 s	Stable δ and ωₘ	Pre-fault steady-state
1–8 s	Voltage collapse, oscillations	Fault causes torque imbalance
8+ s	δ diverges ±180°	Generator loses synchronism
Key Learnings & Concepts

Critical Clearing Time (CCT) estimation

Governor and Excitation system coordination

Dynamic modeling of synchronous generators

Per-unit analysis & dq transformation

 Software & Skills

MATLAB/Simulink (Simscape Electrical)

Power System Dynamics

Transient Fault Analysis

Control System Design

Grid Stability & Damping Theory

 Next Phase

Implement a Power System Stabilizer (PSS) to enhance damping and improve stability after faults.
This demonstrates deeper understanding of advanced control in power systems.




Experience with MATLAB/Simulink

Strong control and machine theory background
