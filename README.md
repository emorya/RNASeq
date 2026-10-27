# Single-Cell RNA-seq: Pancreas and Thymus

A computational analysis of single-cell RNA sequencing data from mouse pancreas and thymus tissues in the **Tabula Muris** dataset.

## Research question

How do pancreas and thymus cells compare in their gene-expression patterns, and which clusters or genes warrant closer examination across the two tissues?

## Analysis

The project notebook explores:

- Loading and combining pancreas and thymus gene-count matrices and matching cell metadata
- Filtering cells by library size and filtering genes by detection frequency
- Library-size normalization
- Principal component analysis (PCA) to explore tissue differences and gene expression
- PhenoGraph and K-means clustering, followed by UMAP visualization
- Examining expression patterns for genes including *Ins1*, *Ins2*, *Gcg*, *Sst*, *Ppy*, *Cd4*, *Cd69*, *Aire*, and *Pdx1*

The notebook describes an initial combined matrix of **3,541 cells** (1,961 pancreas and 1,580 thymus) and **23,433 genes** before subsequent filtering.

## Interpretation and limitations

This is an exploratory student research analysis. The notebook discusses clusters containing cells from both tissues and candidate expression patterns; these observations should not be interpreted as proof of shared cell identity or biological mechanism without additional validation.

## Running the notebook

The original analysis was developed in **Google Colab** with Python and uses `pandas`, `numpy`, `scprep`, `scikit-learn`, `umap-learn`, `phenograph`, `graphtools`, and `matplotlib`.

The notebook expects three input files in Google Drive:

- `Pancreas-counts.csv`
- `Thymus-counts.csv`
- `metadata_FACS.csv`

These datasets are **not included** in this repository. Update the input paths to match your own authorized copies of the data. The notebook has not been packaged as a fully reproducible environment.

## Source and attribution

Data source: [Tabula Muris](https://tabula-muris.ds.czbiohub.org/). The original notebook contains literature references and exploratory interpretation.

## Author

Emory Adelman — computational biology coursework, 2025.
