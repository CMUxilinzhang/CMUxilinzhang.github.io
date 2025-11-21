---
title: "Motor Design Optimization"
excerpt: >
  A nonlinear optimization framework for maximizing torque in compact motors under thermal and geometric constraints.<br/>
  <img src="/images/motor.jpeg">
collection: portfolio
---


## Introduction  
High-torque, compact electric motors are essential for **robot manipulators, exoskeletons, and mobile platforms**. Increasing torque often introduces thermal or geometric constraints.  
**Objective:** formulate and solve a nonlinear optimization problem that maximizes torque at thermal current while ensuring manufacturability and safety.

## Methods  
Based on the mathematical model from :contentReference[oaicite:7]{index=7}:
- Decision variables: stator diameter, magnet thickness, stack length, air gap, turns.  
- Objective: maximize **Kt × Imax** (torque constant × thermal current).  
- Constraints: magnetic flux equations, thermal limits, geometric bounds.  
- Tools: numerical solvers and constraint validation over feasible space.

## Results  
- Identified feasible configurations that satisfy all equality and inequality constraints.  
- Observed sensitivity in flux-density and resistive models when parameters approach lower bounds.  
- Proposed safe operational ranges to maintain manufacturability and thermal reliability.

## Discussion  
The work demonstrates how optimization can systematically improve actuator performance. Future improvements include robustness analysis, uncertainty modeling, and integrating real FEM simulations.

## My Contribution  
I implemented constraints, validated feasible points, visualized solution behavior, and contributed to modeling/analysis sections.  
