---
title: "Data and Methods"
permalink: /datamethods/
author_profile: false
---

Data
------

The genotype data comes from the 1000 Genomes Project and contains information on millions of single nucleotide polymorphisms (SNPs), or individual variants of DNA, on chromosome 22. The gene expression data comes from the Geuvadis RNA-sequencing project. Combined, these sources contain genetic data for 421 individuals across five populations: people of Northern and Western European Ancestry from Utah (CEU), Fins (FIN), British (GBR), Toscani (YRI), and Yoruba (YRI). The genome wide association study (GWAS) summary statistics for IBD were obtained from the analysis carried out in the paper Finucane 2015 Nature Genetics.

Methods
------

As seen above, first the genotype data is extracted with Plink. Then this extracted data, the gene expression data, and the population data are fed into the TWAS/FUSION software to calculate model weights for each gene, where heritability of each feature is estimated. The models used are the linear model that regresses SNPs on gene expression, Lasso Regularization, and ElasticNet, as seen below:
