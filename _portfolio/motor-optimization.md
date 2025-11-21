---
title: "Electric Motor Design Optimization"
excerpt: "Nonlinear constrained optimization of torque under thermal and electromagnetic limits."
collection: portfolio
---

# Electric Motor Design Optimization

This project formulates electric motor design as a **nonlinear constrained optimization problem** aimed at maximizing torque density while respecting electromagnetic and thermal constraints.  
The work enables the design of **compact, high-performance actuators** used in robotic manipulators, exoskeletons, and mobile platforms.

## Objective
Optimize key motor geometric and electromagnetic parameters—including stator diameter, stack length, magnet thickness, air-gap distance, and coil turns—to maximize torque at the allowable thermal current.

## Method
We developed a full electromagnetic–thermal analytical model with:
- torque constant formulation  
- flux density & coil geometry constraints  
- thermal current inequality limits  
- physical manufacturability bounds  

We analyzed:
- constraint geometry  
- feasible region smoothness  
- sensitivity of torque to geometric parameters  

The final nonlinear program was solved using constrained optimization techniques (SQP, interior-point).

## Results
The solver successfully discovered feasible motor configurations that satisfy all constraints while improving torque output.  
Sensitivity results revealed key geometric factors influencing torque constant, resistance, and thermal limits.

## My Role
I contributed to:
- full mathematical modeling  
- constraint formulation  
- feasibility region analysis  
- interpreting optimization results  
