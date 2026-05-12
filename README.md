# AST425 Pulsar Scintillation Parameter Analysis

This repository contains scientific computing workflows and analysis pipelines developed for an AST425 research project focused on pulsar scintillation parameter inference using simulated and observational data.

## Project Overview

The project examines methods for extracting physically significant parameters from pulsar scintillation data using dynamic and secondary spectra. The process involves signal processing, Fourier-transform-based analysis, parameter estimation, statistical validation, and scientific visualization.

Two primary analysis pipelines are included:

- A simulated-data pipeline used to validate parameter-inference methods on synthetic datasets.
- A real-data pipeline used to analyze observational pulsar scintillation data.

## Scientific Background

Pulsars are rapidly rotating neutron stars that emit periodic radio signals. As these signals travel through the interstellar medium, they are scattered by ionized material in space, producing interference patterns known as scintillation.

This project investigates methods for analyzing these scintillation patterns using dynamic and secondary spectra in order to infer physically meaningful parameters related to the scattering geometry and signal propagation.

The workflows developed in this repository focus on:
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
- Fourier-transform-based analysis
- Grid-search parameter estimation
- Monte Carlo Sampling simulations
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
- Screens
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
