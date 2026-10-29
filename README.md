<p align="center">
  <img src="assets/images/logo.png" alt="Scenario exposure logo" width="400" />
</p>

# Scenario exposure

Library for calculating probability density function using various ways.
There is also functionality to sample from the distributions.

## Example

An example script demonstrating how to use the `KDEModel` and `NFModel` classes is
provided in [`example_kde_nf_comparison.py`](example_kde_nf_comparison.py). It samples
points (100, 500, and 2000) from a standard 2D distribution and estimates the density
using both Kernel Density Estimation (KDE) and Normalizing Flows (NF), plotting the
results for comparison. Run it with:

```bash
uv run example_kde_nf_comparison.py
```

## Contributing

- **Run linter:**  

  ```bash
  uv run ruff format . --check  # Remove --check flag to reformat files.
  uv run ruff check .

- **Run typechecking:**

  ```bash
  uv run pyright
  uv run mypy src tests
  ```

- **Run tests:**  

  ```bash
  uv run pytest -s --cov=scenario_exposure --cov-report=term-missing --typeguard-packages=scenario_exposure
  ```

## Acknowledgements
This package is developed as part of the [SYNERGIES project](https://synergies-ccam.eu/).

<img src="assets/images/synergies.svg" alt="SYNERGIES logo" width="300" />


Funded by the European Union. Views and opinions expressed are however those of the author(s) only and do not necessarily reflect those of the European Union or European Climate, Infrastructure and Environment Executive Agency (CINEA). Neither the European Union nor the granting authority can be held responsible for them.


<img src="assets/images/funded_by_eu.svg" alt="Funded by EU logo" width="300" />
