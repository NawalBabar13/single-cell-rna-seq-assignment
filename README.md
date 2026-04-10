# Single-Cell RNA-seq Analysis
Single-cell RNA-seq assignment covering 10X preprocessing, Scanpy analysis, and AnnData


**Course:** Special Topics in Bioinformatics  
**Assignment Type:** Individual  
**Due Date:** 19th April 2026  

---

## Overview

This repository contains the complete workflow for single-cell RNA sequencing (scRNA-seq) data analysis. The pipeline is divided into three sections, each covering a key stage — from raw data preprocessing all the way to downstream analysis and understanding the data format used throughout.

The three sections follow a logical pipeline:

> **Raw 10X Data → Preprocessing → Analysis → Data Structure (AnnData)**

Each section has its own sub-folder containing the relevant notebooks, outputs, and a detailed README.

---

## Section 1: Pre-processing of 10X Single-Cell RNA Datasets

Raw single-cell RNA sequencing data from 10X Genomics cannot be analyzed directly — it first needs to be preprocessed to produce a clean gene expression count matrix. This section follows the Galaxy Training Network tutorial to perform quality control, filtering, and alignment of raw reads.

**Key steps covered:**
- Loading raw 10X FASTQ data
- Quality control and filtering of cells and genes
- Generating a count matrix for downstream analysis

📁 [Go to Section 1 →](./01_preprocessing/)

---

## Section 2: Basic scRNA-seq Analysis with Scanpy

Once we have a clean count matrix from Section 1, this section performs the core single-cell analysis using the Scanpy Python library. This includes identifying distinct cell populations and visualizing them.

**Key steps covered:**
- Normalization and log transformation
- Dimensionality reduction (PCA, UMAP)
- Clustering and marker gene identification
- Cell type annotation

📁 [Go to Section 2 →](./02_scrna_analysis/)

---

## Section 3: AnnData Data Structure

Throughout this pipeline, data is stored in the AnnData (Annotated Data) format — the standard format used by Scanpy and the broader scverse ecosystem. This section covers how AnnData works, how to read/write `.h5ad` files, and how to manipulate the data structure.

**Key steps covered:**
- Understanding the AnnData object structure
- Reading and writing `.h5ad` files
- Slicing, filtering, and annotating AnnData objects

📁 [Go to Section 3 →](./03_anndata/)

---

## Repository Structure

├── README.md

├── 01_preprocessing/

│   └── README.md

├── 02_scrna_analysis/

│   └── README.md

└── 03_anndata/

└── README.md



---

## Tools & Libraries Used

- [Galaxy Project](https://usegalaxy.org/) — cloud-based bioinformatics platform
- [Scanpy](https://scanpy.readthedocs.io/) — single-cell analysis in Python
- [AnnData](https://anndata.readthedocs.io/) — annotated data format for scRNA-seq
