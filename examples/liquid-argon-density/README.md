# Liquid argon example used in the manuscript.

## Manifest

* `reproduce.sh` - bash script to install and configure identical conda environment, run simulations, and generate figures in publication
* `simulate.py` - generate simulation data using OpenMM
* `analyze.py` - analyze simulation data and generate figures in publication
* `cleanup.sh` - bash script to clean up all simulation data and conda environment in preparation for reproducing everything from scratch
* `equilibration.py` - utility methods for computing statistical inefficiencies and determining the equilibration time start usable from other codes

## Dependencies

Installation of dependencies via the `reproduce.sh` bash script requires the [`conda` Python package management tool](http://conda.pydata.org/docs/), which also comes as part of the amazingly useful [Anaconda Scientific Python distribution](https://store.continuum.io/cshop/anaconda/).

## Notes

Note that random number seeds are not hard-coded, so statistical variation among simulation runs will lead to slight variations in the appearance in figures, but should not lead to significant differences in confidence intervals.
