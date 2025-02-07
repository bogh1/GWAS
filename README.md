Genome-Wide Association Study (GWAS) 
**Author:** Brian Oghene  

## **Overview**  
This document presents an in-depth Genome-Wide Association Study (GWAS) analysis conducted on a dataset containing **4,000 individuals (2,000 cases & 2,000 controls)** and **306,102 SNPs**. The study applies **quality control (QC), allele frequency analysis, statistical association tests, and visualization techniques** to identify potential genetic variants associated with a given phenotype.  

## **Key Sections**  
1. **Cohort Summary & SNP Overview**  
   - Sample composition (cases, controls, sex distribution, founders).  
   - SNP count and genotyping rate.  

2. **Quality Control (QC) Analysis**  
   - Missing data assessment per individual & SNP.  
   - Filtering of SNPs based on missingness and Hardy-Weinberg Equilibrium (HWE).  

3. **Allele Frequency Analysis**  
   - Calculation of minor allele frequencies (MAF).  
   - Visualization of MAF distribution.  

4. **Association Testing & Multiple Testing Correction**  
   - Logistic regression with and without covariates.  
   - Bonferroni and False Discovery Rate (FDR) corrections.  
   - Identification of statistically significant SNPs.  

5. **Population Stratification & Genomic Inflation Factor (λ)**  
   - Evaluation of potential population structure effects.  
   - Genomic control adjustment for inflation.  

6. **Manhattan & QQ Plot Analysis**  
   - Visualization of GWAS results.  
   - Identification of significant SNPs associated with the phenotype.  

## **Key Findings**  
- **Significant SNPs Identified:** Multiple SNPs in **TCF7L2** and **FTO** genes were associated with metabolic traits such as **Type 2 Diabetes Mellitus (T2DM) and obesity**.  
- **Genomic Inflation Factor (λ) ~1.01:** Minimal population stratification observed, indicating a well-controlled dataset.  
- **High Genotyping Rate (~98.3%)** suggests minimal missing data, supporting robust statistical analysis.  

## **Tools & Commands Used**  
- **Software:** PLINK, R (ggplot2, qqman)  
- **Commands:**  
  - SNP filtering (`--geno`, `--hwe`)  
  - Missingness analysis (`--missing`)  
  - Logistic regression (`--logistic --adjust`)  
  - Association testing (`--assoc`)  
  - Multiple testing correction (`p.adjust` in R)  

## **References**  
Relevant literature citations on TCF7L2 and FTO gene variants associated with T2DM and obesity are included.  

