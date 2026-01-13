# oyster-flow-graph-code
Reproducible code for  oyster flow graph analysis used in the associated manuscript.
# Oyster Flow Graph (OFG) — Reproducible Code (Notebook)

This repository provides the analysis code used in the manuscript (under review).  
The main executable artifact is a Jupyter/Colab notebook:

- `oysterFlow_en.ipynb`

The notebook implements:
1. Data loading from Google Drive (Colab workflow)
2. Flow-network / stream products generation (WhiteboxTools)
3. Raster-based feature extraction and modeling (Random Forest)
4. Optional clustering & map visualization (KMeans + basemap)

---

## 1. Recommended Environment

### Option A (Recommended): Google Colab
The notebook is written for Colab and includes:
- Google Drive mounting
- `pip install` commands for missing dependencies

### Option B: Local Jupyter
You can also run locally if you adapt file paths (currently hard-coded to Colab/Drive paths).

---

## 2. Dependencies

The notebook uses (non-exhaustive):
- `numpy`, `pandas`
- `matplotlib`
- `rasterio`
- `networkx`
- `scikit-learn`
- `tqdm`
- `whitebox` (WhiteboxTools wrapper)

Optional (for the clustering + basemap visualization cell):
- `geopandas`, `shapely`, `pyproj`, `contextily`

In Colab, the notebook installs key packages via:
```bash
pip install rasterio
pip install whitebox
pip install geopandas shapely pyproj contextily
