# Genome-wide Association Identifies Novel Etiological Insights Associated with Parkinson’s Disease in African and African Admixed Populations 

`GP2 ❤️ Open Science 😍`

**Last Updated:** April 2023 

## Summary
These are all the analyses for the manuscript: ***"Genome-wide Association Identifies Novel Etiological Insights Associated with Parkinson’s Disease in African and African Admixed Populations"***

---
### Analysis Notebooks and Scripts
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
