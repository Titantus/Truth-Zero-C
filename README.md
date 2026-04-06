# T0C Lattice Simulator

Lightweight Python simulation for predicting material properties from lattice geometry and detuning parameters.

## Overview
This project implements a geometric routing model that maps lattice angles and mismatch parameters to observable properties such as:
- Optical transparency vs. opacity
- Selective reflection / pigment behavior
- Thermal routing and phonon dissipation

Built with Python, NumPy, Pandas, and Plotly. Runs entirely in Colab.

## Key Features
- Computes routing efficiency (η) from three detuning parameters: Δθ (angular), Δχ (cloud), Δf (frequency)
- Visualizes coherence cliffs and carrier windows (photons, phonons, conduction)
- Interactive sweeps for fin/lattice angles and transparency predictions
- Reproduces qualitative trends for known materials (diamond transparent, graphite opaque, Cu/Au selective reflection)

## Repository Contents
- `Torque_Routing.ipynb` — Main simulation notebook with dashboard and sweeps
- Supporting visualizations (transparency maps, pigment engine, fin-array results, high-pressure anomalies)

## How to Run
1. Open `Torque_Routing.ipynb` in Google Colab
2. Run all cells — the notebook loads the registry and generates the 4-panel dashboard + sweeps
3. Modify `theta_range` or material parameters in the sweep sections for custom experiments

## Use Cases Explored
- Predicting transparency windows in aluminum-based lattices (sapphire/ALON analogs)
- Mapping phonon (heat) vs photon (transparency) routing as a function of angle
- Rapid virtual screening of lattice geometries for thermal or optical applications

## Technologies
Python • NumPy • Pandas • Plotly • Colab

## Status
Active personal project. Open to collaboration on materials screening or thermal routing extensions.

Feedback and contributions welcome.
