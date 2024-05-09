# Andes_Virus_SC-analysis
Scripts for analysis of single-cell data in Kuzmin et al. 2024


Jupyter notebooks provided for analysis of scRNA-seq and BCR-seq data, using outputs from running Cell Ranger on raw .fastq files from associated GEO entry.

1. preprocessing_concatenation.ipynb : Loading and preprocessing gene expression data, followed by concatenation, dimensionality reduction, and clustering. This generates anndata object for use in other 2 scripts.
2. compositional_analysis_GEX.ipynb : Perform ScCODA analysis, along with DGE, and gene set enrichment.
3. BCR_analysis.ipynb : Analysis of VDJ data using Scirpy.

It is recommended to set up a Conda environment with the 3 main packages below:
* Scanpy (https://scanpy.readthedocs.io/en/stable/) for scRNA-seq analysis
* scCODA (https://github.com/theislab/scCODA) for compositional analysis
* dandelion (https://github.com/zktuong/dandelion) for BCR analysis

Other packages used include Pandas, Numpy, and Matplotlib and Seaborn for plotting
