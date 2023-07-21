[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7652533.svg)](https://doi.org/10.5281/zenodo.7652533)


# Data & code repository for *A pseudoproxy emulation of the PAGES 2k database using a hierarchy of proxy system models*

This repository includes the pseudoPAGES2k dataset described in the paper entitled *A pseudoproxy emulation of the PAGES 2k database using a hierarchy of proxy system models* along with the Jupyter notebooks illustrating the usage of the dataset.

The reference climate input used to generate the pseudoproxies is from the isotope-enabled Community Earth System Model (iCESM) last millennium plus historical simulations ([Brady et al., 2019](https://doi.org/10.1029/2019MS001663)), and the post-processed files can be downloaded here: https://atmos.washington.edu/~rtardif/LMR/prior/


## Download

The pseudoPAGES2k dataset includes multiple versions with various settings.
Please click the links below to download a specific version.

| Dataset ID                                     | Signal              | Noise       | SNR  | Sampling  |
|------------------------------------------------|---------------------|-------------|------|-----------|
| [ppwn_SNRinf_rta](https://github.com/fzhu2e/paper-pseudoPAGES2k/raw/main/data/ppwn_SNRinf_rta.nc)   | psm generated       | none        | inf  | realistic |
| [ppwn_SNR10_rta](https://github.com/fzhu2e/paper-pseudoPAGES2k/raw/main/data/ppwn_SNR10_rta.nc)     | psm generated       | white noise | 10   | realistic |
| [ppwn_SNR2_rta](https://github.com/fzhu2e/paper-pseudoPAGES2k/raw/main/data/ppwn_SNR2_rta.nc)       | psm generated       | white noise | 2    | realistic |
| [ppwn_SNR1_rta](https://github.com/fzhu2e/paper-pseudoPAGES2k/raw/main/data/ppwn_SNR1_rta.nc)       | psm generated       | white noise | 1    | realistic |
| [ppwn_SNR0.5_rta](https://github.com/fzhu2e/paper-pseudoPAGES2k/raw/main/data/ppwn_SNR0.5_rta.nc)   | psm generated       | white noise | 0.5  | realistic |
| [ppwn_SNR0.25_rta](https://github.com/fzhu2e/paper-pseudoPAGES2k/raw/main/data/ppwn_SNR0.25_rta.nc) | psm generated       | white noise | 0.25 | realistic |
| [ppwn_SNRinf_fta](https://github.com/fzhu2e/paper-pseudoPAGES2k/raw/main/data/ppwn_SNRinf_fta.nc)   | psm generated       | none        | inf  | full      |
| [ppwn_SNR10_fta](https://github.com/fzhu2e/paper-pseudoPAGES2k/raw/main/data/ppwn_SNR10_fta.nc)     | psm generated       | white noise | 10   | full      |
| [ppwn_SNR2_fta](https://github.com/fzhu2e/paper-pseudoPAGES2k/raw/main/data/ppwn_SNR2_fta.nc)       | psm generated       | white noise | 2    | full      |
| [ppwn_SNR1_fta](https://github.com/fzhu2e/paper-pseudoPAGES2k/raw/main/data/ppwn_SNR1_fta.nc)       | psm generated       | white noise | 1    | full      |
| [ppwn_SNR0.5_fta](https://github.com/fzhu2e/paper-pseudoPAGES2k/raw/main/data/ppwn_SNR0.5_fta.nc)   | psm generated       | white noise | 0.5  | full      |
| [ppwn_SNR0.25_fta](https://github.com/fzhu2e/paper-pseudoPAGES2k/raw/main/data/ppwn_SNR0.25_fta.nc) | psm generated       | white noise | 0.25 | full      |
| [tpwn_SNR10_rta](https://github.com/fzhu2e/paper-pseudoPAGES2k/raw/main/data/tpwn_SNR10_rta.nc)     | nearest temperature | white noise | 10   | realistic |
| [tpwn_SNR2_rta](https://github.com/fzhu2e/paper-pseudoPAGES2k/raw/main/data/tpwn_SNR2_rta.nc)       | nearest temperature | white noise | 2    | realistic |
| [tpwn_SNR1_rta](https://github.com/fzhu2e/paper-pseudoPAGES2k/raw/main/data/tpwn_SNR1_rta.nc)       | nearest temperature | white noise | 1    | realistic |
| [tpwn_SNR0.5_rta](https://github.com/fzhu2e/paper-pseudoPAGES2k/raw/main/data/tpwn_SNR0.5_rta.nc)   | nearest temperature | white noise | 0.5  | realistic |
| [tpwn_SNR0.25_rta](https://github.com/fzhu2e/paper-pseudoPAGES2k/raw/main/data/tpwn_SNR0.25_rta.nc) | nearest temperature | white noise | 0.25 | realistic |
| [tpwn_SNR10_fta](https://github.com/fzhu2e/paper-pseudoPAGES2k/raw/main/data/tpwn_SNR10_fta.nc)     | nearest temperature | white noise | 10   | full      |
| [tpwn_SNR2_fta](https://github.com/fzhu2e/paper-pseudoPAGES2k/raw/main/data/tpwn_SNR2_fta.nc)       | nearest temperature | white noise | 2    | full      |
| [tpwn_SNR1_fta](https://github.com/fzhu2e/paper-pseudoPAGES2k/raw/main/data/tpwn_SNR1_fta.nc)       | nearest temperature | white noise | 1    | full      |
| [tpwn_SNR0.5_fta](https://github.com/fzhu2e/paper-pseudoPAGES2k/raw/main/data/tpwn_SNR0.5_fta.nc)   | nearest temperature | white noise | 0.5  | full      |
| [tpwn_SNR0.25_fta](https://github.com/fzhu2e/paper-pseudoPAGES2k/raw/main/data/tpwn_SNR0.25_fta.nc) | nearest temperature | white noise | 0.25 | full      |

## Usage

Jupyter notebooks illustrating the usage of the dataset leveraging `cfr` v2023.7.21 (`pip install cfr==2023.7.21`, DOI: [10.5281/zenodo.7855587](https://doi.org/10.5281/zenodo.7855587)):

- [Loading and visualization](./notebooks/pdb-load-viz.ipynb)
- [Database Filtering](./notebooks/pdb-filter.ipynb)
- [Validation Dashboards](./notebooks/dashboards.ipynb)
- [PPE: A PDA-based Reconstruction](./notebooks/ppe-pda.ipynb)


## How to cite
This repository can be cited with DOI: [10.5281/zenodo.7652533](https://doi.org/10.5281/zenodo.7652533)