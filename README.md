# Insights Into Parkinson's Disease Genetics in African Populations

## Expanded GWAS Identifies Ancestry-Specific and Cross-Population Risk Loci

`GP2 ❤️ Open Science 😍`

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) 

DOI: Pending

**Last Updated:** March 2026

------------------------------------------------------------------------

## Overview

This repository accompanies the manuscript: **"Insights Into Parkinson's Disease Genetics in African Populations: Expanded GWAS Identifies Ancestry-Specific and Cross-Population Risk Loci"**

This study represents the argest genome-wide association study (GWAS)
of Parkinson's disease (PD) in African (AFR) and African-admixed (AAC)
populations to date. We integrated individual-level genotype data from the Global
Parkinson's Genetics Program (GP2; release 11) with summary statistics from
23andMe and the Million Veterans Program (MVP) to better
characterize the genetic architecture of PD in underrepresented
populations.

### Summary
* Integrated GP2, 23andMe, and Million Veterans Program data (3,975 cases, 319,883 controls), conducting separate and combined GWAS in African and African admixed ancestry populations prior to meta-analysis
* Key findings confirm and extend known risk loci: 
  * GBA1 (rs3115534) was the top signal across all analyses
  * SNCA and SCARB2 replicated as trans-ancestry loci
  * a novel LRRK2 coding variant (p.T1410M) reached genome-wide significance in AFR populations for the first time, alongside two additional novel loci.

### Citation
If you use this repository or find it helpful for your research, please cite the corresponding manuscript:
> **Insights Into Parkinson's Disease Genetics in African Populations: Expanded GWAS Identifies Ancestry-Specific and Cross-Population Risk Loci**
>
> by Okubadejo et al., Global Parkinson's Genetics Program (GP2)
> 
> medRxiv 2026; DOI: xx

------------------------------------------------------------------------

## Important Note About the 2023 Paper

If you are looking for the original analyses corresponding to:

> *Rizig et al., 2023: "Genome-wide Association Identifies Novel Etiological Insights Associated with Parkinson's Disease in African and African Admixed Populations"*

please use the **`main` branch** of this repository, found here: https://github.com/GP2code/GP2-AFR-AAC-metaGWAS/tree/main. The **current branch contains the expanded 2026 analyses** and should be cited for the new manuscript.


## Data Statement
Data used in the preparation of this article were obtained from GP2. Specifically, we used Tier 2 data from GP2 (release 11; DOI 10.5281/zenodo.17753486). GP2 data can be accessed through AMP PD (https://amp-pd.org). For the MVP dataset, PD summary statistics from the Million Veteran's Program (MVP) were downloaded from dbGAP (accession number: phs002453.v1.p1; analysis accession: pha010400.1). Summary statistics from 23andMe were shared under a collaborative agreement, submitted at https://research.23andme.com/collaborate/. 

## Helpful Links

-   GP2 Website: https://gp2.org/
-   GP2 Cohort Dashboard: https://gp2.org/cohort-dashboard-advanced/
-   GP2 Introduction Paper:
    https://movementdisorders.onlinelibrary.wiley.com/doi/10.1002/mds.28494
-   GP2 Publications:
    https://pubmed.ncbi.nlm.nih.gov/?term=%22global+parkinson%27s+genetics+program%22

------------------------------------------------------------------------

## Workflow Overview

![Workflow
Diagram](https://github.com/GP2code/GP2-AFR-AAC-metaGWAS/blob/2026/figures/workflow.png)


------------------------------------------------------------------------

## Repository Structure
```
.
├── analyses
│   ├── 00_Prepping_Data.ipynb
│   ├── 01_Covariates.ipynb
│   ├── 02_GWAS_GP2.ipynb
│   ├── 03_Munge_Sumstats.ipynb
│   ├── 04_Meta_Analysis.ipynb
│   ├── 05_Manhattans_QQs.ipynb
│   ├── 06_Calculate_Lambdas.ipynb
│   ├── 07_AA_AFR_Blood.ipynb
│   └── 08_Forest_Plots.ipynb
├── figures
│   └── workflow.png
├── LICENSE
├── README.md
└── tables
```

------------------------------------------------------------------------

## Analysis Notebooks

Languages: Python, R, and Bash

| Notebook             | Description                                             |
| -------------------- | ------------------------------------------------------- |
| 00_Prepping_Data     | Harmonization, phenotype cleaning, and sample filtering |
| 01_Covariates        | Making of covariate file (sex and PCs)                  |
| 02_GWAS_GP2          | Cohort-level GWAS in GP2                                |
| 03_Munge_Sumstats    | Formatting and QC of summary statistics                 |
| 04_Meta_Analysis     | AFR, AAC, and combined meta-analyses                    |
| 05_Manhattans_QQs    | Manhattan and QQ plots                                  |
| 06_Calculate_Lambdas | Genomic inflation and QC metrics                        |
| 07_AA_AFR_Blood      | Blood-specific follow-up analyses                       |
| 08_Forest_Plots      | Cross-cohort forest plots                               |


## Software

| Software              | Version(s) | URL                                                                                            | RRID       | Notes                     |
| --------------------- | ---------- | ---------------------------------------------------------------------------------------------- | ---------- | ------------------------- |
| ANNOVAR               | 2020-06-08 | [http://www.openbioinformatics.org/annovar/](http://www.openbioinformatics.org/annovar/)       | SCR_012821 | Variant annotation        |
| METAL                 | 2020-05-05 | [http://csg.sph.umich.edu/abecasis/Metal/](http://csg.sph.umich.edu/abecasis/Metal/)           | SCR_002013 | Meta-analysis             |
| PLINK                 | 1.9, 2.0   | [http://www.nitrc.org/projects/plink](http://www.nitrc.org/projects/plink)                     | SCR_001757 | Genetic analyses          |
| Python                | 3.9+       | [http://www.python.org](http://www.python.org)                                                 | SCR_008394 | pandas, numpy, matplotlib |
| R                     | 4.2+       | [http://www.r-project.org](http://www.r-project.org)                                           | SCR_001905 | tidyverse, data.table     |



------------------------------------------------------------------------

## Acknowledgments

This work was performed on behalf of the Global Parkinson's Genetics
Program (GP2). We thank all study participants, clinicians, and contributing cohorts
worldwide.
