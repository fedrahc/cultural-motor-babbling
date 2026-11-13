# Modeling Cultural Motor Babbling

Independent research project (Oct-Nov 2026).

## Question

If caregivers followed feedback regimes parameterized from cross-cultural data, what would a simple learner acquire about its own body, and which parameters matter most?

This project does not test whether culture shapes infant development. It asks what follows in a simple model when the feedback regime changes.

## Model (planned)

- **Learner:** a simulated 2-joint planar arm that babbles and learns a forward model (joint angles -> hand position).
- **Caregiver:** a fixed, rule-based feedback function. Regimes differ only in their config file.
- **Conditions:** control (no feedback), distal-style, proximal-style.
- **Metrics:** forward-model error on a fixed test grid, workspace coverage, divergence between learned models.

## Structure

- `docs/evidence_map.csv`: each model parameter, its value, its source and how strong the evidence is
- `configs/`: one YAML file per condition
- `src/cmb/`: arm, learner, caregiver, metrics, experiment runner
- `tests/`: sanity tests
- `results/`: raw outputs (not committed) and figures

## Status

Work in progress. Limitations and future work will be listed here.
