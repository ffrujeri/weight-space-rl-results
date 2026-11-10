# Astra weight programming: control experiments and observability

Published results: https://felipefrujeri.dev/weight-space-rl-results/

This repository contains a standalone results page for from-random control
experiments on Pendulum, Hopper, Walker2d, HalfCheetah, Humanoid, and Microduck.

The newest section reports Microduck's completed full-feedback/no-feedback Astra
comparison against equal-budget PPO and constant-bias search, plus a larger native
PPO reference. It includes command-conditioned motion, survival, training/candidate
curves, and recovery of Astra's three-parameter ankle controller. A state-feedback
removal test separates controller feedback from its fixed bias. The initial
baseline audit is preserved below. All studies disclose their single-seed limits
and distinguish balance from commanded locomotion.

The HalfCheetah and Humanoid section reports completed comparisons against
SAC at 36,864 interactions, with 100 held-out resets per policy, training curves,
and numerical forecasts committed before Astra received candidate feedback.
It reports prediction errors against a persistence reference and distinguishes
Humanoid's short survival from reliable locomotion.

The observability section traces what Astra changed in the seed-7 Walker2d controller.
It includes the eight submissions, exact compact-controller recovery, component
removal tests on 20 fresh shared resets, and two observability figures. It
distinguishes measured policy behavior from unknown internal model representations.

The ablation study compares 12 fresh Astra editors given full trajectories,
step rewards only, episode returns only, or no environment feedback. The report
includes held-out results, all candidate curves, uncertainty, and behavior
diagnostics. No-feedback curves are audits measured after commitment.

The original Astra-versus-CleanRL-SAC comparison is preserved below as historical
context. It supplied richer physics information and used a different protocol.
These experiments are single-seed feasibility pilots; they do not establish a general
ranking across algorithms or feedback types.

`index.html` embeds its figures and requires no external assets or login.
Open it locally, or use the GitHub Pages link above. GitHub Pages publishes
from the root of the `main` branch.

Latest addition: [Microduck controller-family search](https://felipefrujeri.dev/weight-space-rl-results/#microduck-gain-search), with fresh held-out tests, all development candidates, and protocol limitations.
