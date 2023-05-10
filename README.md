# ws-remoras

This repository contains analysis code and data relating to Whitehead et al. (2023) in which we used [SLEAP](https://sleap.ai) to track remoras and whale sharks from drone footage during feeding epochs.

## Setup

Create the environment with:
```
conda env create -f environment.yml && conda activate ws-remoras
```

To add it as a Jupyter/IPython kernel:
```
python -m ipykernel install --user --name ws-remoras
```

## Usage
All the source data is self-contained here in the [`data`](data) folder (tracking, analysis outputs), raw movies in [`videos`](videos), figures in [`figs`](figs), and visualization movies in [`viz`](viz).

To regenerate any figures or movies, run the following notebooks in order:
1. [`analysis.ipynb`](analysis.ipynb): This will plot and save static figures.
2. [`make_egocentric_movies.ipynb`](make_egocentric_movies.ipynb): This will egocentrize the poses (align everything to the whale sharks in standard coordinates) and generate visualization movies.
3. [`egocentric_analysis.ipynb`](egocentric_analysis.ipynb): Supplementary analyses (some not included in the paper) on the egocentric data.

## Citation
```
Whitehead et al. (2023)  # TODO: Update when full citation available.
```
