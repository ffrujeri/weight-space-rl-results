# Astra vs SAC: results from random initialization

Published results: https://ffrujeri.github.io/weight-space-rl-results/

This repository contains the standalone results page for a three-environment
control pilot comparing direct weight programming by Astra with CleanRL SAC.
Both methods start with identical random actor tensors and are compared at
matched online interaction budgets.

The report includes held-out results, training and development curves, protocol,
limitations, and suggested follow-up experiments. It is a one-seed feasibility
study with substantial physics knowledge available to Astra, not a general
claim that weight editing outperforms reinforcement learning.

`index.html` embeds its figures and requires no external assets or login.
Open it locally, or use the GitHub Pages link above. GitHub Pages publishes
from the root of the `main` branch.
