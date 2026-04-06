# **T0C Lattice Simulator**

Lightweight Python simulation for predicting material properties from lattice geometry and detuning parameters.

## **Overview**
This project implements a geometric routing model that maps lattice angles and mismatch parameters to observable behaviors such as:

- optical transparency vs. opacity  
- selective reflection and pigment behavior  
- thermal routing and phonon dissipation  

The simulator is built with Python, NumPy, Pandas, and Plotly, and runs entirely in Google Colab.

## **Core Workflow — The Truth Requirement**
The simulator uses a simple epistemic tagging system to keep assumptions honest and prevent over‑extrapolation:

- **⧉ Observable** — measured or simulated data  
- **⧠ Model‑Established** — internally consistent behavior  
- **⇢ Derived Prediction** — logical consequence awaiting validation  
- **→ ? Potential** — unverified continuation beyond the current resolution  

This workflow does not reject assumptions; it labels them so that corrections become calibration events rather than hidden errors.

## **Key Features**
- Computes routing efficiency (η) from three detuning parameters:  
  - Δθ (angular detuning)  
  - Δχ (cloud mismatch)  
  - Δf (frequency clash)  
- Visualizes coherence cliffs and routing windows  
- Interactive sweeps for lattice angles and transparency predictions  
- Reproduces qualitative trends for known materials:  
  - diamond transparent  
  - graphite opaque  
  - Cu/Au selective reflection  

## **Repository Contents**
- **Torque_Routing.ipynb** — main simulation notebook with dashboard and sweeps  
- **/docs/T0C.md** — full logic specification and epistemic tagging rules  
- Supporting visualizations (transparency maps, pigment engine, high‑pressure anomalies)

## **How to Run**
1. Open `Torque_Routing.ipynb` in Google Colab  
2. Run all cells — the notebook loads the registry and generates the dashboard  
3. Modify `theta_range` or material parameters for custom experiments  

## **Use Cases Explored**
- Predicting transparency windows in aluminum‑based lattices (sapphire/ALON analogs)  
- Mapping phonon vs. photon routing as a function of angle  
- Rapid virtual screening of lattice geometries for optical or thermal applications  

## **Technologies**
Python • NumPy • Pandas • Plotly • Colab

## **Status**
Active personal project.  
Open to collaboration on materials screening, routing models, or thermal‑optical simulations.
