# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a
Changelog](https://keepachangelog.com/en/1.1.0/), and this project adheres to
[Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [v0.1.1](https://github.com/mlcast-community/mlcast-dataset-radklim/releases/tag/v0.1.1)

### Fixed

- Rain variable `RR` renamed as `rainfall_amount` to match `standard_name` (`rainfall_amount`) and units (`kg m-2`) present in source netcDF files.
- Adapt `mlcast` specific meta information to match requirements of `mlcast-dataset-validator@0.1.0`

### Maintenance

- Update `pre-commit` version to ensure compatability with `python3.14` used in github ci

## [v0.1.0](https://github.com/mlcast-community/mlcast-dataset-radklim/releases/tag/v0.1.0)

First tagged release of zarr version of the RadKlim dataset including both hour
and 5-minute data, and up to Extension 6 (so that the total timespan covered is
2001-2023). Includes fixes to projection `crs_wkt` string to set x/y coord
units correctly (as `km` rather than `m`) and domain bounds (which are required
when `cartopy` when using the projection for plotting).
