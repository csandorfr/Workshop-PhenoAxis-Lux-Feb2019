# Phenotypic axes Analysis Workshop: CENTRE-PD Consortium Meeting (Luxembourg), February 2019

This repository contains course materials for the phenotipic analysis workshop at CENTRE-PD Consortium Meeting (Luxembourg), February 2019

Download or clone the repository so that you have everything you need to participate in the course.

## Course materials

This repository contains data files and RMarkdown documents that can be used for the analysis of the datasets. The clinical observations used here come from the PPMI cohort and the original data can be downloaded here: 

**Data file:** 

* Clinical data must be downloaded data from the PPMI database in compliance with the PPMI Data Use Agreement. 

**Rmd file:**

There is RMarkdown document including a "complete" version with full R code. 

* Data analysis: `Workshop_Luxembourg_Phenotypic_Axes.Rmd`


**HTML file:**

HTML reports produced by running the above ("complete") Rmd files in case you want to check the expected code output and plots.

* `Workshop_Luxembourg_Phenotypic_Axes.html`

The above should give you everything you need to work along with the analyses in the workshop. 

## PHENIX

You will need to download here and install the R package PHENIX 

```{r}
wget https://mathgen.stats.ox.ac.uk/genetics_software/phenix/phenix_1.0.tar.gz
R CMD INSTALL ./phenix_1.0.tar.gz
```
## Others R packages

You will need to have the following R packages installed: `ggplot2`,`reshape2`,`sva`. We will use the development versions of the Bioconductor packages.

```{r}
install.packages(c("ggplot2","reshape2"))
## try http:// if https:// URLs are not supported
if (!requireNamespace("BiocManager", quietly = TRUE))
install.packages("BiocManager")
BiocManager::install("sva")
```

## Useful Resources

* `PHENIX publication` : A multiple-phenotype imputation method for genetic studies
https://www.nature.com/articles/ng.3513

* `PHENIX software`: PHENotype Imputation eXpediated
https://mathgen.stats.ox.ac.uk/genetics_software/phenix/phenix.html

* `PPMI cohort`: The Parkinson’s Progression Markers Initiative orginal data
https://www.ppmi-info.org/

