# Mathematical Modeling of Cigarette and E-Cigarette Use Using Delay Differential Equations

## Overview
This project models cigarette and e-cigarette use across different age groups using a modified Susceptible-Infected-Recovered (SIR) model with Delay Differential Equations (DDEs).

The model incorporates delayed initiation, quitting, and relapse to study how nicotine use changes over time.

## Methodology
- Divides the population into three age groups: youth, young adults, and adults.
- Uses nine compartments representing susceptible, current users, and recovered individuals.
- Incorporates three time delays:
  - Initiation: 12 months
  - Recovery: 6 months
  - Relapse: 12 months
- Models time-varying initiation (β), recovery (γ), and relapse (ρ) rates.
- Includes birth, death, and aging transitions between population groups.
- Simulates cigarette and e-cigarette use over a 10-year period.
- Compares predicted youth e-cigarette use with CDC-reported data for 2023 and 2024.
- Tests parameter sensitivity by varying β, γ, and ρ by ±10%.

## Code
`NicotineUse_SIR_DDE_Model.ipynb` contains the mathematical model, numerical simulations, population projections, sensitivity analysis, and visualizations.

The notebook includes initial drafts, the final model, and experimental analysis sections.

## Requirements
Python, NumPy, Pandas, Matplotlib, ddeint, Seaborn, and GeoPandas.

The notebook can be run in Google Colab.

## Outputs
The analysis generates:
- Cigarette and e-cigarette use projections by age group
- Susceptible, current-user, and recovered population trends
- Comparisons between model predictions and CDC data
- Sensitivity analysis plots for initiation, recovery, and relapse rates
- Heatmaps and U.S. state-level nicotine use visualizations

The projections depend on the model's assumed parameters and initial conditions.
