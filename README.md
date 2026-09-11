# SVC-reproducibility

Code used to reproduce the analyses and figures in the SVC manuscript.

Main SVC software repository: https://github.com/aster-ww/SVC

Processed data and model checkpoints are available on Zenodo: https://doi.org/10.5281/zenodo.22693727

## Setup

Two paths are resolved from environment variables, both defaulting to two levels above the
notebook (`../..`), which is where they sit when this repository is cloned inside the SVC tree:

- `SVC_ROOT` — the main SVC repository, for `import svc` (Figures 2, 4, 5)
- `SVC_DATA_ROOT` — the processed data from Zenodo, unpacked as `<SVC_DATA_ROOT>/<dataset>/`

```bash
git clone https://github.com/aster-ww/SVC.git
export SVC_ROOT=/path/to/SVC
export SVC_DATA_ROOT=/path/to/data
```

## Structure

```
SVC-reproducibility/
├── fig2/                         # reproduces Figure 2
│   ├── precomputed/              # files read by the notebook
│   └── fig2_reproducibility.ipynb
├── fig3/                         # reproduces Figure 3
│   ├── precomputed/              # files read by the notebook
│   └── fig3_reproducibility.ipynb
├── fig4/                         # reproduces Figure 4
│   ├── precomputed/              # files read by the notebook
│   └── fig4_reproducibility.ipynb
└── fig5/                         # reproduces Figure 5
    ├── precomputed/              # files read by the notebook
    └── fig5_reproducibility.ipynb
```
