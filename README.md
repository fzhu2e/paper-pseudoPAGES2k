[![DOI](https://zenodo.org/badge/DOI/10.1038/s41597-023-02489-1.svg)](https://doi.org/10.1038/s41597-023-02489-1)
[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7652533.svg)](https://doi.org/10.5281/zenodo.7652533)


# Data & code repository for *A pseudoproxy emulation of the PAGES 2k database using a hierarchy of proxy system models*

This repository includes the pseudoPAGES2k dataset described in the paper published in *Scientific Data*:

    Zhu, F., Emile-Geay, J., Anchukaitis, K.J. et al. A pseudoproxy emulation of the PAGES 2k database using a hierarchy of proxy system models. Sci Data 10, 624 (2023). https://doi.org/10.1038/s41597-023-02489-1

along with the Jupyter notebooks illustrating the usage of the dataset.


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

If you use the pseudoPAGES2k dataset in your scientific publication, we would appreciate using the following citations:


```bibtex
@article{Zhu2023SciData,
  title = {A Pseudoproxy Emulation of the {{PAGES}} 2k Database Using a Hierarchy of Proxy System Models},
  author = {Zhu, Feng and {Emile-Geay}, Julien and Anchukaitis, Kevin J. and McKay, Nicholas P. and Stevenson, Samantha and Meng, Zilu},
  year = {2023},
  month = sep,
  journal = {Scientific Data},
  volume = {10},
  number = {1},
  pages = {624},
  publisher = {{Nature Publishing Group}},
  issn = {2052-4463},
  doi = {10.1038/s41597-023-02489-1},
  urldate = {2023-09-14},
  copyright = {2023 Springer Nature Limited},
  langid = {english},
  keywords = {Palaeoceanography,Palaeoclimate},
}

@dataset{feng_zhu_2023_8173256,
  author       = {Feng Zhu and
                  Julien Emile-Geay and
                  Kevin J. Anchukaitis and
                  Nicholas P. McKay and
                  Samantha Stevenson and
                  Zilu Meng},
  title        = {The pseudoPAGES2k Dataset v1.4},
  month        = jul,
  year         = 2023,
  publisher    = {Zenodo},
  version      = {v1.4},
  doi          = {10.5281/zenodo.8173256},
  url          = {https://doi.org/10.5281/zenodo.8173256}
}
```