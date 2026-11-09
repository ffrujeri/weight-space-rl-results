# Astra weight programming: feedback ablation and SAC comparison

Published results: https://felipefrujeri.dev/weight-space-rl-results/

This repository contains the standalone results page for two control studies
on Pendulum, Hopper, and Walker2d, starting from random actor weights.

The latest study compares 12 fresh Astra editors given full trajectories,
step rewards only, episode returns only, or no environment feedback. The report
includes held-out results, all candidate curves, uncertainty, and behavior
diagnostics. No-feedback curves are audits measured after commitment.

The original Astra-versus-CleanRL-SAC comparison is preserved below as historical
context. It supplied richer physics information and used a different protocol.
Both studies are single-seed feasibility pilots; they do not establish a general
ranking across algorithms or feedback types.

`index.html` embeds its figures and requires no external assets or login.
Open it locally, or use the GitHub Pages link above. GitHub Pages publishes
from the root of the `main` branch.
