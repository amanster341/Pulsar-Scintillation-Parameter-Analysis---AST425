# AST425 Pulsar Scintillation Parameter Analysis

This repository contains a scientific computing research project and analysis pipelines focusing on pulsar scintillation parameter inference using simulated and observational data.

## Project Overview

The project examines methods for extracting physically significant parameters from pulsar scintillation data using dynamic spectra, which show signal intensity as a function of time and observing frequency, and secondary spectra, which reveal underlying scattering features after Fourier-transform-based processing. The process involves signal processing, parameter estimation, statistical validation, and scientific visualization.

In the research project, two primary analysis pipelines are included:

- A simulated-data pipeline used to validate parameter-inference methods on synthetic datasets.
- A real-data pipeline used to analyze observational pulsar scintillation data.

## Project Goals

The main goal of this project was to recover phase-related parameters, including "A" and "δ", from scintillation features in the secondary spectrum from a binary pulsar system. "A" represents an orbital drift-related parameter that describes how the scintillation pattern shifts over an orbit, while "δ" represents a phase-offset parameter. Recovering these parameters helps constrain the scattering geometry and can contribute to improved pulsar distance estimates.

The simulated-data pipeline was used to test whether the method could recover known input parameters. In contrast, the real-data pipeline applied the same approach to observational data where the true parameters were unknown. Constraining these parameters can help improve estimates of pulsar distance and scattering geometry. In binary pulsar systems, improved distance and geometric constraints can support broader studies of neutron star physics, including the high-density equation of state.

The analysis involved selecting strong signal regions in the secondary spectrum, searching over a grid of possible parameter values, identifying the strongest power response, and using repeated Monte Carlo trials to estimate the stability of the inferred results.

## Scientific Background

Pulsars are rapidly rotating neutron stars that emit periodic radio signals. As these signals travel through the interstellar medium, they are scattered by ionized material in space, producing interference patterns known as scintillation. Furthermore, pulsars and neutron stars are among the densest objects in the universe, making them ideal candidates to study the properties of matter under high density, otherwise known as the equation of state. 

This project investigates methods for analyzing these scintillation patterns using dynamic and secondary spectra in order to infer physically meaningful parameters related to the scattering geometry and signal propagation.

The work developed in this repository focuses on:
- processing simulated and observational pulsar data,
- extracting signal features from secondary spectra,
- performing parameter inference using grid-search and Monte Carlo methods,
- and validating results through repeated statistical analysis.

## Repository Structure

```text
AST425-MAIN_WORK/
├── README.md
├── requirements.txt
├── notebooks/
├── figures/
├── data/
└── archive/

```

## Methods and Techniques

- Python scientific computing
- Data handling and processing
- Data adaptation and pipeline construction
- Fourier-transform-based analysis
- Grid-search parameter estimation
- Monte Carlo simulations
- Signal processing
- Scientific visualization
- Statistical analysis and uncertainty estimation

## Software and Libraries

- Python
- NumPy
- Pandas
- Matplotlib
- Astropy
- SciPy
- Screens/scintillation simulation tools
- Jupyter Notebook

## Notes

This project builds upon research methods and reference notebooks provided within the AST425 research environment. The final analysis pipelines were adapted, restructured, debugged, validated, and extended for this project.

Large observational datasets and intermediate outputs are not fully included in this repository.

## Future Improvements

Potential future additions include:
- Improved documentation and workflow organization
- Containerized environments using Docker
- Automated workflows and reproducibility improvements
- Expanded visualization and parameter-analysis tools
