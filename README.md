# Computational Physics & Signal Processing Projects

This repository contains four Jupyter notebooks showcasing projects in **computational physics** and **data science**. The notebooks explore a wide range of phenomena, including fractal growth, statistical mechanics, social modeling, and gravitational wave signal processing.

---

## 1. Diffusion-Limited Aggregation (DLA)  
**File:** `1. Diffusion-limited Aggregation.ipynb`

This notebook simulates **Diffusion-Limited Aggregation (DLA)**, a process in which particles undergoing random walks (Brownian motion) irreversibly cluster together to form complex, fractal-like structures.

### Key Concepts
- Random walks  
- Fractal growth  
- Fractal dimension  

### Methodology
- Initialize a grid with a central seed particle.
- Simulate particles performing random walks until they attach to the growing cluster.
- Compute the fractal dimension \( D \) by analyzing the scaling relation between the number of particles \( N \) and the cluster radius \( R \).

### Visualizations
- Scatter plots of cluster growth realizations  
- Log–log plots used to estimate the fractal dimension  

---

## 2. The Ising Model  
**File:** `2. Ising Model.ipynb`

This notebook explores the **Ising Model**, a foundational model of ferromagnetism in statistical mechanics. The system is simulated using the **Metropolis–Hastings Monte Carlo algorithm** to study phase transitions in a lattice of magnetic spins.

### Key Concepts
- Phase transitions  
- Curie temperature  
- Monte Carlo methods  
- Magnetization  

### Methodology
- Initialize a 2D lattice of spins (\(+1\) or \(-1\)).
- Apply the Metropolis algorithm to update spins based on energy minimization and thermal fluctuations.
- Compute thermodynamic observables:
  - Energy \( E \)
  - Magnetization \( M \)
  - Specific heat \( C_v \)

### Visualizations
- Grid-based visualizations of spin domains  
- Magnetization vs. temperature plots illustrating the phase transition  

---

## 3. Schelling’s Model of Segregation  
**File:** `3. Schelling's Model.ipynb`

An implementation of **Schelling’s Model of Segregation**, an agent-based model demonstrating how local preferences for similar neighbors can lead to large-scale social segregation—even when individual agents are relatively tolerant.

### Key Concepts
- Agent-based modeling  
- Emergent behavior  
- Segregation index  

### Methodology
- Create a 2D grid populated with two types of agents and empty spaces.
- Agents relocate if the fraction of neighboring agents of the same type falls below a tolerance threshold \( p \).
- Use 2D correlation (`scipy.signal.correlate2d`) to efficiently compute neighborhood similarity.

### Visualizations
- Color-coded grids showing the evolution from a mixed state to segregated clusters  

---

## 4. Gravitational Wave Signal Processing  
**File:** `4. Signal_Processing_Gravitational_waves.ipynb`

This notebook focuses on **digital signal processing techniques** used to detect and analyze **gravitational waves**, with an emphasis on events such as the **GW170817 neutron star merger**.

### Key Concepts
- Fourier transforms  
- Spectrograms and Q-transforms  
- Signal-to-noise ratio (SNR)  

### Methodology
- Load strain data from LIGO’s Hanford and Livingston detectors.
- Apply whitening and bandpass filtering to suppress noise.
- Generate time–frequency representations to visualize the characteristic gravitational-wave “chirp.”

### Visualizations
- Time-series plots of raw and filtered strain data  
- Spectrograms highlighting the frequency sweep during the merger  

---

## Requirements

To run these notebooks, the following Python libraries are required:

- `numpy`  
- `matplotlib`  
- `scipy`  
- `tqdm` — progress bars for simulations  
- `gwpy` — required for the gravitational wave analysis notebook  

---
