---
permalink: /
title: "Application of Transcriptome-Wide Association Studies to Find Genes that are Associated with Inflammatory Bowel Disease"
excerpt: "About me"
author_profile: false

---

Samuel Zhou, Jacqueline Lee, Esha Desai, Moksha Poladi

The work displayed in this webiste was conducted under the supervision of Tiffany Amariuta-Bartell.

The code for this project can be located [here](https://github.com/jacquelinekclee/twas-dsc180-a17). Our full report can be located here.

Introduction
======
Understanding how genetic variation impacts gene expression can help us identify gene-based mechanisms of disease risk. For the last two decades, genome-wide association studies (GWAS) were utilized to identify disease-associated genetic variants. However, these associated variants often do not lie in gene exons, creating uncertainty as to which genes are associated with disease. Our project aims to fill this gap by leveraging a technique known as transcriptome-wide association studies (TWAS). TWAS is a powerful strategy that can detect gene–trait associations if variation in the expression of a gene colocalizes with phenotypic variation. It combines expression quantitative trait locus (eQTL) data with GWAS summary statistics to identify disease-associated genes. We leverage gene expression and genotype data from the 1000 Genomes project and GWAS from UK Biobank. Here, we focused our analysis on Inflammatory Bowel Disease. Ultimately, the identification of disease-associated genes will accelerate the development of therapeutics and treatment options for patients.

Background
======
As seen above, the diseased population may have one variant of DNA (AA), and the non-diseased population may have a different one (AT). The AA in the diseased population's DNA may lead to increased transcripts of a particular gene, which in turns leads to the presence of the disease. Identifying these gene-based mechanism of disease risk is crucial to facilitate early diagnosis and treatment of individuals. Previous approaches attempted to understand this mechanism by detecting key variants associated with gene expression, which in turn is responsible for regulating the production of certain key proteins that can lead to the presence of certain diseases[<sup>1</sup>](https://notsamzhou.github.io/twas/references/). For example, GWAS finds thousands of trait-associated variants, however, 93% of disease and trait-associated variants emerging from these studies lie within noncoding sequences of the DNA[<sup>2</sup>](https://notsamzhou.github.io/twas/references/).  It is infeasible to measure gene expression in as many people that are in a GWAS cohort. This also makes it difficult to understand the functionality of these variants and their association with disease risk.

What is TWAS and Why is it Important?
------
For our project, we decided to use a technique called TWAS that aggregates variant effects of gene expression and estimates a gene level association[<sup>3</sup>](https://notsamzhou.github.io/twas/references/). TWAS aims to identify genes that lead to manifestation of complex human traits due to genetically regulated transcriptional activity[<sup>4</sup>](https://notsamzhou.github.io/twas/references/). It integrates genome-wide association studies (GWAS) and gene expression datasets to identify gene–trait associations . TWAS leverages eQTL cohorts with expression and genotype data to discover gene–trait associations from GWAS summary statistics. The eQTL cohort is then used to find predictive models of gene expression by using allele counts of genetic variants in the gene’s vicinity[<sup>5</sup>](https://notsamzhou.github.io/twas/references/). The model is then used to impute the genetic component of gene expression in a large sample of people with genotyping results (ex. a GWAS cohort). Finally, TWAS correlates the disease phenotype and predicts gene expression to find disease associated genes[<sup>6</sup>](https://notsamzhou.github.io/twas/references/). Ultimately TWAS is powerful in identifying the disease associated gene by aggregating the effects of multiple variants into a single testing unit[<sup>3</sup>](https://notsamzhou.github.io/twas/references/). Identification of a gene, rather than just a variant, can enable scientists to create drugs targeting a specific gene that can potentially offset or mitigate the effects of the associated disease.

The Disease of Interest: IBD
------
Inflammatory Bowel Disease (IBD) is a highly heritable disease, which causes a chronic inflammation of tissues in an individual’s digestive tract[<sup>7</sup>](https://notsamzhou.github.io/twas/references/). This disease affects 3.1 million adults in the United States and adversely impacts their quality of life[<sup>8</sup>](https://notsamzhou.github.io/twas/references/). Even though GWAS has identified hundreds of variants associated with Inflammatory Bowel Disease (IBD), there are few known associated genes. For our project we decided to leverage TWAS to identify the genes associated with IBD. To this end, we collected gene expression data in the blood because IBD is an immune disease and blood will contain the relevant cell types. We also collected GWAS summary statistics.

---

[Back to top](#top)
