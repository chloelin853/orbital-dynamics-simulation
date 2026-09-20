# Orbital Dynamics Simulation

**Chloe Lin · University College London · Python scientific computing**

**A plausible orbit is not enough: check what the numerical method conserves.**

Implemented Euler, velocity Verlet and RK4 for gravitational motion, then explored more complex three-body configurations in the original project (2025).

![New circular-orbit demonstration: identical initial conditions, timestep 0.02 and duration 40 in dimensionless units. Energy errors are shown on a logarithmic scale.](figures/integrator_comparison.png)

*New circular-orbit demonstration: identical initial conditions, timestep 0.02 and duration 40 in dimensionless units. Energy errors are shown on a logarithmic scale.*

**[Start the guided notebook](notebooks/main_analysis.ipynb)** · [Detailed logbooks](notebooks/logbooks) · [Presentation provenance](docs/PRESENTATION_NOTES.md)

## What this demonstrates

- Numerical integration, physical diagnostics, and interpreting timestep-dependent error.
- A runnable three-method comparison against an analytic circular orbit.
- Links to the original 27 triple-star parameter combinations and simplified 500-year Alpha Centauri investigation.

In this short benchmark, RK4 has very small error and Verlet has bounded energy oscillations; Euler drifts substantially. This is not a claim that one method is universally best.

## Scope

No external dataset is needed. The guided notebook includes analytic convergence and angular-momentum checks. Original three-body outputs are historical; close-encounter results need further timestep checks. The Alpha Centauri example is a simplified model, not a precision prediction.

## Run the guided notebook

From the repository root, create and activate a Python virtual environment, then:

```sh
python -m pip install -r requirements-demo.txt
python -m jupyter lab notebooks/main_analysis.ipynb
```

The short notebook has saved outputs for browsing and runnable cells that regenerate the opening figure. It supports a working directory of either the repository root or `notebooks/`. The original project dependencies are listed separately in `requirements.txt`.

## Repository map

```text
README.md
notebooks/
  main_analysis.ipynb      # Start here
  logbooks/               # Original detailed work
figures/                  # Generated README figure
docs/                     # Review and provenance notes
requirements-demo.txt      # Guided notebook
requirements.txt           # Original project dependencies
```


## Status and attribution

Private working draft; visibility will change only at Chloe's request. The guided notebook is a new presentation of the project, and does not validate all historical results. Original sources and teaching-material references remain in the logbooks. Confirm sharing conditions before publication; no open-source licence has been selected.
