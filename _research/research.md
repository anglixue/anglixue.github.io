---
layout: archive
title: "Research"
permalink: /research/
author_profile: true
---

{% include base_path %}


<small>(updated to 08-NOV-2023)</small>

<br>

Research Interests
======
I am generally interested in understanding the genetic basis of complex diseases by applying existing and developing novel statistical and computational tools on large-scale bulk/single-cell datasets.

<br>

Current Research
======

* Curating the largest single-cell multi-omics cohort (TenK10K) which profiles the scRNA-seq data of ~50 million peripheral blood mononuclear cells from ~10,000 individuals 
* Identifying genetic variants associated with intra-individual variance on the gene expression level (sc-veQTL)
* Integrating multi-omics data to discover novel biomarkers for autoimmune diseases by using causal inference techniques
* Utilising gene regulatory network and single-cell eQTL mapping to unveil causal genes for autoimmune diseases

<br>

Past Research
======      

<strong><u>Single-cell pseudo-bulk eQTL mapping</u></strong>

I evaluated the pitfalls and opportunities for applying latent variables in single-cell eQTL analyses. In the eQTL association analysis, people typically infer latent variables from the expression matrix and incorporate the inferred variables as covariates in the association model to remove unwanted variations. However, in recent studies published by our lab, it was found that the number of detected eGenes dropped with the incremental increase of PEER factors (Yazar et al. Science. 2022; Neavin et al. Genome Biology. 2021). I dug into this issue and found that the loss of power is due to the unique data structure of the single-cell pseudo-bulk matrix (including sparsity, skewness, and mean-variance relationship). **I proposed a series of quality controls and a novel algorithm to decide the number of latent variables adjusted in the association model.**

Citation: **Angli Xue#**, Seyhan Yazar, Drew Neavin, Joseph E. Powell#. "Pitfalls and opportunities for applying latent variables in single-cell eQTL analyses". ***Genome Biology***. 24.1 (2023): 1-11. (# corresponding author) [[full text](https://genomebiology.biomedcentral.com/articles/10.1186/s13059-023-02873-5)]

<strong><u>GWAS and post-GWAS</u></strong>

This work collected ~700,000 individuals (the largest in the world at that time) and performed GWAS to uncover 42 genetic variants associated with type 2 diabetes. I used a multi-omics integration technique and prioritised 33 putative functional genes for T2D, where genetic variants are associated with T2D risk mediated by altering gene expression levels. **I further incorporated DNA methylation data and highlighted 3 genes (CAMK1D, TP53INP1, and ATP5G1) with plausible regulatory mechanisms, whereby a genetic variant exerts an effect on T2D through epigenetic regulation of gene expression**. The study provides a flexible framework that is applicable to any complex trait to discover the biological mechanisms of GWAS loci. 

Citation: **Angli Xue**, Yang Wu, Zhihong Zhu, Futao Zhang, Kathryn E Kemper, Zhili Zheng, Loic Yengo, Luke R. Lloyd-Jones, Julia Sidorenko, Yeda Wu, eQTLGen Consortium, Allan F McRae, Peter M Visscher, Jian Zeng, Jian Yang. Genome-wide association analyses identify 143 risk variants and putative regulatory mechanisms for type 2 diabetes. ***Nature Communications***. 12, 6450 (2018). [[full text](https://www.nature.com/articles/s41467-018-04951-w)]

<strong><u>Population Genetics</u></strong>

Previous studies have found conflicting evidence of the relationship between alcohol consumption and cardiovascular traits (Griswold et al. The Lancet. 2018; Liu et al. Nature Genetics. 2019). I provided a plausible explanation for this long-standing controversy about the effects of alcohol consumption on health outcomes in genetic and epidemiological studies. My research pointed out that **the discrepancy was mainly due to the misreports and longitudinal changes (MLC)** in the dataset. I proposed a novel approach to correct the biases by combining medical records and online follow-up questionnaires in the UK Biobank and **almost all the previously reported negative estimates of genetic correlations between alcohol consumption and common diseases become positive/non-significant after the MLC corrections.** I further caution researchers about potential caveats in large-scale genetic studies of behavioural traits. 

Citation: **Angli Xue**, Longda Jiang, Zhihong Zhu, Naomi R. Wray, Peter M. Visscher, Jian Zeng, Jian Yang. Genome-wide analyses of behavioral traits are subject to bias by misreports and longitudinal changes. ***Nature Communications***. 12, 6450 (2021). [[full text](https://www.nature.com/articles/s41467-020-20237-6)]

<strong><u>Causal Inference</u></strong>

I benchmarked 11 Mendelian Randomisation (MR) methods for causal inference between two traits and co-developed an improved version of [GSMR](https://yanglab.westlake.edu.cn/software/gcta/#GSMR) software. **The improved version included a global heterogeneity testing algorithm to detect and filter directional pleiotropic effects that could potentially bias the causal effect estimation.** I highlighted the challenges that are more specific to MR analysis in substance use behaviours. By integrating stratified regression, genetic correlation, and MR analyses, I found evidence of dosage-dependent effects of coffee and tea intake on common diseases (e.g., cardiovascular disease and osteoarthritis). I also for the first time identified a top GWAS signal (rs4410790, near the AHR gene) for tea intake level that showed opposite effects on heavy and moderate tea intake.

The software has been made into both R and C++ version and released in the Github repository. 
[[R package: GSMR2](https://github.com/jianyanglab/gsmr2)]
[[C++ version: GCTA-GSMR](https://github.com/jianyangqt/gcta)]

Citation: **Angli Xue**, Zhihong Zhu, Huanwei Wang, Longda Jiang, Peter M. Visscher, Jian Zeng, Jian Yang. Unravelling the complex causal effects of substance use behaviours on common diseases. ***Communications Medicine***. Accepted in Principle. [Preprint](https://www.researchsquare.com/article/rs-3465061/v1)


