# Section 1: Pre-processing of 10X Single-Cell RNA Datasets

## Overview
This section covers the preprocessing of raw 10X Genomics single-cell RNA-seq data using the Galaxy platform. Raw FASTQ reads are aligned, quantified, and filtered to produce a high-quality gene expression count matrix.

## Tools Used
- **RNA STARsolo** — alignment and gene expression quantification
- **DropletUtils** — filtering of empty droplets to produce a clean count matrix
- **MultiQC** — quality control report

## Steps Performed
1. Imported raw FASTQ files (2 lanes, R1 + R2) from Zenodo
2. Imported genome annotation (GTF) and cell barcode whitelist
3. Ran RNA STARsolo to align reads and generate raw count matrix
4. Ran DropletUtils (DefaultDrops) to filter for ~300 high quality cells
5. Generated MultiQC report for quality assessment

## Output Files
| File | Description |
|------|-------------|
| `*.tsv` (Barcodes) | Filtered cell barcodes |
| `*.tsv` (Genes) | Gene list |
| `*.mtx` (Matrices) | Sparse count matrix |
| `MultiQC*.html` | Quality control report |
