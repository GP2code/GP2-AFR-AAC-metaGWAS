# Genome-wide Association Identifies Novel Etiological Insights Associated with Parkinson’s Disease in African and African Admixed Populations 

`GP2 ❤️ Open Science 😍`

[![DOI](https://zenodo.org/badge/635483971.svg)](https://zenodo.org/badge/latestdoi/635483971)

**Last Updated:** April 2023 

## Summary
This is the online repository for the manuscript titled ***"Genome-wide Association Identifies Novel Etiological Insights Associated with Parkinson’s Disease in African and African Admixed Populations"***. This study represents the first and largest genome-wide assessment of Parkinson’s disease in the African and African admixed populations.

### Helpful Links 
- BioRxiv pre-print *(in preparation)*
- [GP2 Website](https://gp2.org/)
    - [GP2 Cohort Dashboard](https://gp2.org/cohort-dashboard-advanced/)
- [Introduction to GP2](https://movementdisorders.onlinelibrary.wiley.com/doi/10.1002/mds.28494)
    - [Other GP2 Manuscripts (PubMed)](https://pubmed.ncbi.nlm.nih.gov/?term=%22global+parkinson%27s+genetics+program%22)


# Workflow Diagram 
![Workflow Diagram](https://github.com/GP2code/GP2-AFR-AAC-metaGWAS/blob/main/figures/F1_Workflow.png)



# Repository Orientation 
- The `analyses/` directory includes all analyses discussed in the manuscript
- The `figures/` directory includes all figures and supplemental figures referenced in the manuscript *(pending publication)*
- The `tables/` directory includes all tables and supplemental tables referenced in the mansucript *(pending publication)*

---
### Analysis Notebooks
* Languages: Python, bash, and R

| **Notebooks** |                                                    **Description**                                                   |
|:----------------:|:--------------------------------------------------------------------------------------------------------------------:|
|        00_Prepping_Data    | Cleaning data and generating covariate files |
|        01_perGroup_GWASes  | Running GWASes per group (no indels, age, sex, PCs 1-10 as covariates) |
|        02_formatMETAL      | Format additive summary statistics for meta-GWASes with METAL |
|        03_AAC_ONLY_META    | Meta-GWAS #1: Looking at African admixed individuals only |
|        04_AFR_ONLY_META    | Meta-GWAS #2: Looking at African individuals only |
|        05_AFR_AAC_Combined_META  | Meta-GWAS #3: Looking at African and African admixed individuals |
|        06_Investigate_Hits  | Investigating the top hits from the joint meta-GWAS |
|        07_BetaBeta_Plots    | Generating beta-beta plots |
|        08_Zygosity_rs3115534  | Get the zygosity distribution of individuals for rs3115534 |
|        09_Manhattan_QQ_Plots  | Visualize the meta-GWASes |
|        10_Compare_GWASes_NallsFooKim | Seeing the number of variants from the previously identified 104 that show up in our meta-GWAS |
|        11_PRS_Nalls2019_90_EUR-GLM  | Conducting PRS on cohorts: Pulling the 90 European variants from Nalls et al., 2019 and using European betas |
|        12_PRS_23andMe_90_EUR-GLM  | Conducting PRS on cohorts: Pulling the 90 European variants from Nalls et al., 2019 and using AAC betas from 23andMe summary statistics |
|        13_adHoc_Analyses | Runs of homozygosity, linear regression for % admixture and age, haplotypes with 1KG, fine-mapping, dominant vs recessive modeling, annotating WGS for T2, conditional analysis, Miami plot compared to Europeans, and GBA Gauchian caller WDL |

---
### Figures and Supplemental Figures

*(pending publication)*

---
### Tables and Supplemental Tables 

*(pending publication)*

---

# Software 

|               Software              |      Version(s)     |                       Resource URL                       |       RRID      |                                               Notes                                               |
|:-----------------------------------:|:-------------------:|:--------------------------------------------------------:|:---------------:|:-------------------------------------------------------------------------------------------------:|
|               ANNOVAR               |      2020-06-08     |        http://www.openbioinformatics.org/annovar/        | RRID:SCR_012821 |                refGene; avsnp150; ljb26_all; gnomad312_genome; used for annotation                |
|                coloc                |       5.1.0.1       | https://cran.r-project.org/web/packages/coloc/index.html |       N/A       |                                  R package; used for fine-mapping                                 |
|         GBA Gauchian caller         |        1.0.2        |           https://github.com/Illumina/Gauchian           |       N/A       |   Illumina's targeted variant caller for the GBA gene based on a whole-genome sequencing (WGS)    |
|                METAL                |      2020-05-05     |         http://csg.sph.umich.edu//abecasis/Metal/        | RRID:SCR_002013 |                                       used for meta-analyses                                      |
|                PLINK                | 1.7 and 1.9 and 2.0 |            http://www.nitrc.org/projects/plink           | RRID:SCR_001757 |                                     used for genetic analyses                                     |
|     Python Programming Language     |     3.8 and 3.9     |                  http://www.python.org/                  | RRID:SCR_008394 | pandas; numpy; seaborn; matplotlib; statsmodel; used for general data wrangling/plotting/analyses |
| R Project for Statistical Computing |         4.2         |                 http://www.r-project.org/                | RRID:SCR_001905 |   tidyverse; dplyr; tidyr; ggplot; data.table; used for general data wrangling/plotting/analyses  |
