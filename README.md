# Calculated Fractal Dimension of Time-Series Data
This repository contains Python implementations for calculating the fractal dimension of various time-series data using Spectral Exponent, Hurst Exponent, and Higuchi’s Algorithm. The analysis is inspired by the paper "Fractal Dimension Algorithms and Their Application to Time Series Associated with Natural Phenomena" by F. Cervantes-De la Torre et al. (2013).

## Overview
Fractal dimensions are vital for characterizing the self-similarity and scaling behavior of non-linear time-series data. This repository applies three distinct methods to compute fractal dimensions:

- **Spectral Analysis:** Computes the spectral exponent(𝛽) to characterize the frequency domain behavior.
- **Hurst Exponent:** Measures long-term memory effects and trends in the data.
- **Higuchi’s Algorithm:** Calculates fractal dimensions directly from the time series.
## Applications
These methods are used to analyze time-series data associated with natural phenomena, such as geomagnetic disturbances, to gain insights into the dynamics and scaling behaviors of such systems.

## Files and Contents
### Notebooks
- **Hurst_Exponent.ipynb**
Contains the implementation for calculating the Hurst Exponent using rescaled range analysis.

- **Fractal_Dimension.ipynb**
Implements Higuchi’s Algorithm and Spectral Analysis to compute fractal dimensions of the time-series data.

### Research Paper
**la_Torre_2013.pdf:** The reference paper providing theoretical and practical insights into fractal dimension computation techniques.
## Methods Used
  - **Spectral Analysis**
    - Power spectral density(𝑆(𝑓) analysis to determine the spectral exponent (𝛽).
    - Relationship: 𝑆(𝑓)∝𝑓−𝛽.
  - **Hurst Exponent** 
    - Uses rescaled range (R/S) analysis to calculate the Hurst exponent (𝐻):
      - 𝐻=0.5: Random walk (Brownian motion)
      - 𝐻>0.5: Persistent behavior
      - 𝐻<0.5: Anti-persistent behavior
  - **Higuchi’s Algorithm**
    - Directly estimates the fractal dimension (𝐷) of a time series using a time-scaling approach.
    - Relationship: 𝐷=(5−𝛽)/2

## Results
Preliminary analysis demonstrates that:
  - Fractal dimensions effectively reveal scaling properties and dynamics of time series.
  -Higuchi’s method is more robust for non-stationary data compared to spectral and Hurst exponent approaches.
  - The crossover behavior identified using Higuchi’s algorithm indicates shifts in system dynamics.
## Dependencies
  - Python 3.8 or above
  - NumPy
  - SciPy
  - Matplotlib
  - Jupyter Notebook
## Reference
  - Cervantes-De la Torre, F., González-Trejo, J. I., Real-Ramírez, C. A., & Hoyos-Reyes, L. F. (2013). Fractal Dimension Algorithms and Their Application to Time Series Associated with Natural Phenomena. Journal of Physics: Conference Series, 475, 012002. DOI:10.1088/1742-6596/475/1/012002.
