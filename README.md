# *GDCRNATools* - An R package for downloading, organizing, and integrative analyzing lncRNA, mRNA, and miRNA data in GDC


## Introduction

The [Genomic Data Commons (GDC)](https://portal.gdc.cancer.gov/) maintains standardized genomic, clinical, and biospecimen data from National Cancer Institute (NCI) programs including [The Cancer Genome Atlas (TCGA)](https://tcga-data.nci.nih.gov/) and [Therapeutically Applicable Research To Generate Effective Treatments (TARGET)](https://ocg.cancer.gov/programs/target), It also accepts high quality datasets from non-NCI supported cancer research programs, such as genomic data from the [Foundation Medicine](https://www.foundationmedicine.com/).

`GDCRNATools` is an R package which provides a standard, easy-to-use and comprehensive pipeline for downloading, organizing, and integrative analyzing RNA expression data in the GDC portal with an emphasis on deciphering the lncRNA-mRNA related ceRNA regulatory network in cancer.

Many analyses can be perfomed using GDCRNATools, including differential gene expression analysis ([limma](http://bioconductor.org/packages/release/bioc/html/limma.html), [edgeR](http://bioconductor.org/packages/release/bioc/html/edgeR.html), and [DESeq2](http://bioconductor.org/packages/release/bioc/html/DESeq2.html)), univariate survival analysis (CoxPH and KM), competing endogenous RNA network analysis (hypergeometric test, Pearson correlation analysis, regulation similarity analysis, sensitivity Pearson partial  correlation), and functional enrichment analysis(GO, KEGG, DO). Besides some routine visualization methods such as volcano plot, scatter plot, and bubble plot, etc., three simple shiny apps are developed in GDCRNATools allowing users visualize the results on a local webpage.

This user-friendly package allows researchers perform the analysis by simply running a few functions and integrate their own pipelines such as molecular subtype classification, [weighted correlation network analysis (WGCNA)](https://labs.genetics.ucla.edu/horvath/CoexpressionNetwork/Rpackages/WGCNA/), and TF-miRNA co-regulatory network analysis, etc. into the workflow easily.


## Installation
`GDCRNATools` is now under review in Bioconductor. Users can install the package from github temporarily using the `install_github()` function in `devtools` package.

Code to install and load `devtools`:
```R
install.pacakges('devtools')
library(devtools)
```

Code to install and load `GDCRNATools`:
```R
devtools::install_github(repo='Jialab-UCR/GDCRNATools')
library(GDCRNATools)
```

## Manual
A comprehensive manual of `GDCRNATools` is available [GDCRNATools Manual](https://github.com/Jialab-UCR/Jialab-UCR.github.io/blob/master/GDCRNATools_manual.html). Users can download the manual in .html format and view on the local computer or download the manual in .pdf format from here [GDCRNATools Manual](https://github.com/Jialab-UCR/Jialab-UCR.github.io/blob/master/GDCRNATools_manual.pdf). 

