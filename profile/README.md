# tsshape

**Python tools for shaping time-series data.**

---

## About

tsshape is a collection of Python packages for working with time-series data — from ingestion and transformation to validation and export. Our libraries are built to be composable, lightweight, and easy to integrate into data pipelines and analysis workflows.

---

## Packages

| Package | Description | Version |
|---------|-------------|---------|
| [`tsshape`](https://github.com/ts-shape/tsshape) | Core time-series shaping and transformation | ![PyPI](https://img.shields.io/pypi/v/tsshape) |
| [`tsshape-io`](https://github.com/ts-shape/tsshape-io) | Read and write time-series from common formats (CSV, Parquet, JSON) | ![PyPI](https://img.shields.io/pypi/v/tsshape-io) |
| [`tsshape-validate`](https://github.com/ts-shape/tsshape-validate) | Schema definition and validation for time-series datasets | ![PyPI](https://img.shields.io/pypi/v/tsshape-validate) |

---

## Quick Start

```sh
pip install tsshape
```

```python
import pandas as pd
from tsshape import reshape

df = pd.read_csv("sensor_data.csv", parse_dates=["timestamp"])

# Resample, fill gaps, and normalize in one call
result = reshape(df, freq="1min", fill="interpolate", normalize=True)
```

---

## Links

- [GitHub Repositories](https://github.com/orgs/ts-shape/repositories)
- [PyPI](https://pypi.org/org/tsshape)
