---
layout: project
title: Formula Sled Race Simulation
description: A simulation-based CS project modeling sled velocity, rider performance, and training impact.
technologies: [Python, matplotlib, OOP]
image: /assets/images/FIG1.png
---

As part of a computer science course, I developed a simulation framework to analyze performance in a fictional **Formula Sled Race**. The simulation modeled sled runs based on physics principles, incorporating **riders, sled types, and track environments**, all while simulating motion over time using **object-oriented programming** in Python.

The core challenge was to determine **which combination of rider, sled, and training strategy would win the race**, using performance metrics like velocity, distance traveled, and whether the sled completed the track.


We then ran comparative simulations before and after applying training regimens, such as:

```python
# Strengthen all riders and rerun simulations
cardio_training = Cardio_Training(riders, 3)
cardio_training.perform_training()

strength_training = Strength_Training(riders, 6)
strength_training.perform_training()

# Run updated simulations and plot results
for rider in riders:
    sim = Aerolift_Simulation(time_step, rider, aerolift_sled, track)
    sim.run_simulation()
    simulations.append(sim)

Simulation results were visualized using matplotlib, allowing us to compare how different riders, sleds, and tracks performed under identical conditions. This also let us evaluate training benefits numerically and visually.
