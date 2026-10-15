# SVC-reproducibility

Code used to reproduce the analyses and figures in the SVC manuscript.

Preprint: https://doi.org/10.64898/2026.10.07.757371

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

## Citation

Wan, H., Yang, P., Hou, S., Wang, J.X. and Zhou, X. SVC: A Vision Transformer-based Spatially and Virtually Embedded Cell Model for Deciphering Subcellular Spatial Transcriptomic Heterogeneity. *bioRxiv* (2026). https://doi.org/10.64898/2026.10.07.757371

```bibtex
@article{wan2026svc,
  title     = {SVC: A Vision Transformer-based Spatially and Virtually Embedded Cell Model for Deciphering Subcellular Spatial Transcriptomic Heterogeneity},
  author    = {Wan, Hui and Yang, Penghui and Hou, Siyu and Wang, Jade and Zhou, Xiang},
  journal   = {bioRxiv},
  year      = {2026},
  doi       = {10.64898/2026.10.07.757371},
  publisher = {Cold Spring Harbor Laboratory}
}
```
