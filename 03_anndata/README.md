# Section 3: AnnData Data Structure

## Overview
This section covers the AnnData (Annotated Data) format, which is the standard data structure used throughout single-cell RNA-seq analysis in Python. AnnData is the backbone of the scverse ecosystem and is used by Scanpy to store count matrices along with all associated metadata.

## Tools Used
- **AnnData** — annotated data matrix library for Python
- **Google Colab** — cloud-based Jupyter notebook environment

## Steps Performed
1. Created AnnData objects from scratch
2. Explored the structure of AnnData — `X`, `obs`, `var`, `uns`, `obsm`, `varm`
3. Added observations (cell) and variable (gene) annotations
4. Sliced and filtered AnnData objects
5. Read and wrote `.h5ad` files
6. Concatenated multiple AnnData objects

## Output Files
| File | Description |
|------|-------------|
| `getting_started.ipynb` | AnnData getting started notebook with all outputs |

## Key Concepts Learned
- `adata.X` — the main count matrix (cells × genes)
- `adata.obs` — metadata about cells (rows)
- `adata.var` — metadata about genes (columns)
- `adata.uns` — unstructured/additional data
- `adata.obsm` — multi-dimensional cell annotations (e.g. PCA, UMAP coordinates)# Section 3: AnnData Data Structure

