# vehicle-suspension-simulation
Python-based analysis of a 1-DOF mass-spring-damper system, investigating damping, spring stiffness, settling time, and oscillations

# Vehicle Suspension Dynamics & Simulation

A Python-based study investigating how spring stiffness and damping influence the dynamic response of a simplified vehicle suspension system.

## Project Overview

This project uses a linear one-degree-of-freedom (1-DOF) mass-spring-damper model to investigate free vibration and the effects of varying suspension parameters.

The governing equation is:

$$
m\ddot{x} + c\dot{x} + kx = 0
$$

where:
- \(m\) = mass (kg)
- \(c\) = damping coefficient (N·s/m)
- \(k\) = spring stiffness (N/m)
- \(x\) = displacement (m)

## Objectives

- Simulate displacement and velocity responses.
- Investigate how spring stiffness affects oscillation frequency.
- Compare underdamped, critically damped, and overdamped systems.
- Calculate settling times using a 5% tolerance band.
- Evaluate the trade-off between settling time and reverse displacement.

## Tools

- Python
- NumPy
- SciPy (`solve_ivp`)
- Matplotlib
- Jupyter Notebook

## Key Findings

- Increasing spring stiffness increases natural frequency.
- Increasing damping generally reduces oscillations.
- Critical damping provides the fastest non-oscillatory return to equilibrium.
- Excessive damping can increase settling time.
- Damping selection involves balancing response speed and oscillation amplitude.

## Limitations

This project uses a simplified 1-DOF free-vibration model. It does not include road disturbances, tire stiffness, unsprung mass, or experimental validation.

## Future Work

A 3D CAD representation using PTC Creo and a more realistic quarter-car model may be developed as future extensions.
