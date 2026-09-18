# Orbital Dynamics Simulation

An individual computational physics project by Chloe Lin, completed for PHAS0030 at University College London in 2025.

This project uses Python to investigate gravitational two-body and three-body motion, comparing numerical integrators through orbital trajectories, timestep sensitivity, and conservation of energy and angular momentum.

## Notebooks

1. **[Logbook 1](orbital_dynamics_logbook_1.ipynb)**: Euler, velocity Verlet, and fourth-order Runge-Kutta integration; fixed-central-mass and comparable-mass two-body systems; and a star-planet-moon system.
2. **[Logbook 2](orbital_dynamics_logbook_2.ipynb)**: Lagrange's equilateral three-body configuration, initial-velocity variations, a simplified Alpha Centauri model, and a fictional triple-star parameter study.

The repository copies retain the original calculations, commentary, references, and saved figures. Filenames and author headings have been simplified to omit the student identifier. The source notebooks remain unchanged.

## Investigations and observations

- Compared Euler, velocity Verlet, and RK4 using energy and angular momentum diagnostics.
- Observed bounded energy fluctuations with velocity Verlet compared with accumulating Euler drift in the studied examples.
- Explored how initial conditions affect close encounters, scattering, and ejection in three-body systems.
- Investigated 27 combinations of third-star separation, speed, and inclination.
- Modelled a simplified Alpha Centauri configuration over 500 simulated years, comparing the inner binary with and without the third star's influence.

These are coursework simulations with simplifying assumptions, not precision astronomical predictions. Finite-duration trajectories do not establish general long-term stability or instability.

## Setup

Create and activate a Python virtual environment, then install the dependencies:

```sh
python -m pip install -r requirements.txt
python -m jupyter lab
```

Open either notebook. Review Logbook 1 before Logbook 2 for the methodological background. Each notebook should be run in its own fresh kernel, from top to bottom. Some simulations and parameter sweeps may take time.

## Draft status

This is a private working draft. Saved outputs come from the original coursework and have not been regenerated for this repository. Python cell syntax was checked during preparation; a clean execution and numerical validation remain to be completed before public release. Dependencies are not yet version-pinned.

Potential review work includes checking initial conditions, consistent units, conserved-quantity calculations, timestep convergence, and the interpretation of close encounters. Very small plotted variations should be read together with axis offsets and numerical precision.

## Attribution

The original references are retained in the notebooks, including PHAS0030 teaching material and the sources used for the three-body and Alpha Centauri investigations. Confirm any course-material sharing conditions before public release. No open-source licence has been selected at this stage.

The repository will remain private until Chloe requests publication.
