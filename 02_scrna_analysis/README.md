# Section 2: Basic scRNA-seq Analysis with Scanpy

## Overview
This section performs downstream single-cell RNA-seq analysis on a PBMC (Peripheral Blood Mononuclear Cells) dataset using the Scanpy Python library in Google Colab. Starting from a filtered count matrix, the notebook performs quality control, normalization, dimensionality reduction, clustering, and cell type annotation.

## Tools Used
- **Scanpy** — single-cell analysis in Python
- **AnnData** — data structure for storing annotated data matrices
- **Google Colab** — cloud-based Jupyter notebook environment

## Steps Performed
1. Loaded PBMC 3k dataset and created AnnData object
2. Quality control — filtered low quality cells and genes
3. Normalized and log-transformed the count matrix
4. Identified highly variable genes
5. Performed PCA for dimensionality reduction
6. Built neighborhood graph and ran UMAP
7. Performed Leiden clustering to identify cell populations
8. Found marker genes for each cluster
9. Annotated cell types based on marker genes

## Output Files
| File | Description |
|------|-------------|
| `basic-scrna-tutorial.ipynb` | Complete Scanpy analysis notebook with all outputs and plots |

## Key Results
- Successfully identified distinct cell populations in PBMC data
- Generated UMAP visualization showing cell clusters
- Identified marker genes for each cell type including T cells, B cells, NK cells, and monocytes
