# First Part of Thesis - Imputation Methods Comparison
This repository includes the code for the first part of my thesis project in which I analyze different imputation methods in PBMC data.

The original gene expression and surface protein counts of the 10k PBMC’s Dataset from 10X Genomics can be found in this [link](https://www.10xgenomics.com/resources/datasets/10-k-pbm-cs-from-a-healthy-donor-gene-expression-and-cell-surface-protein-3-standard-3-0-0)

To apply the pipeline for analyzing gene expression results, either use the orignal counts or imputed counts, as desired.
- To use MAGIC for the imputation, use the pipeline [MAGIC_Pipeline_analysis.Rmd](MAGIC_Pipeline_analysis.Rmd)
- To use DeepImpute/scGNN for the imputation, use the pipeline [Pipeline_analysis_general.Rmd](Pipeline_analysis_general.Rmd) - follow the instruction of each method on its GitHub page, and upload the imputed CSV file to the pipeline.

** The annotations file used is attached above and needs to be downloaded to the local computer.

To apply the pipeline for analyzing the original gene expression results with the surface protein results, use [raw_data_analysis_with_surface_prot.Rmd](raw_data_analysis_with_surface_prot.Rmd).

To easily reproduce MASKING results here are links to the CSV files of the:
- [Original Gene Expression Counts](https://drive.google.com/file/d/19F8MOrpsPifGa8regRby_wqXFv4wb6W-/view?usp=sharing)
- [Masked Gene Expression Counts](https://drive.google.com/file/d/17gKrnjWsIoQT8pB1ewo5LgcxUb7PJyI1/view?usp=sharing)
- [Imputes Masked counts by MAGIC](https://drive.google.com/file/d/17gKrnjWsIoQT8pB1ewo5LgcxUb7PJyI1/view?usp=sharing)
- [Imputes Masked counts by DeepImpute](https://drive.google.com/file/d/1AekpB9SZFonpy6huj_oGArTqJWYUtWHW/view?usp=sharing) 

** [mask_10__of_data.ipynb](mask_10__of_data.ipynb): code to mask 10% of the data.<br/>
** [analysis_of_Imputated_masked_data.ipynb](analysis_of_Imputated_masked_data.ipynb): code for the analysis of the imputed masked counts.

Quick access to imputation method's GitHub pages :
- [GitHub page - MAGIC](https://github.com/KrishnaswamyLab/MAGIC)
- [GitHub page - DeepImpute](https://github.com/lanagarmire/deepimpute)
- [GitHub page - scGNN](https://github.com/juexinwang/scGNN)
