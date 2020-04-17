In this folder, we present the weights trained from the Framingham Heart Study (off-spring and third-generation cohorts) with a total sample size of 2,441. 

There are a few files with their names begin with:
1. CV_full_weights.tar.gz contains weights trained from CVs-only models
2. Joint_full_weights.tar.gz contains weights trained from joint models (CVs and RVs)
3. RV_full_weights.tar.gz contains weights trained from RVs-only models

After unziping the files, there are multiple .RDat files with the names of genes (official symbol). 

In each .RDat file, there are three components:
1. bimfile: contains the SNP location (hg19), reference allele, and alternative allele
2. R2: contains Rsq based on elastic net models cross-validated with lambda.1se and lambda.min and their corresponding number of cis-eQTLs
3. wgt.matrix: contains weights trained by elastic net regession cross-validated with lambda.1se and lambda.min

For Joint_full_weights files, we further indicate whether an included SNP is a RV and how many RVs are selected in the final model in R2 (nRV_min) and wgt.matrix (rare_ind), respectively.

Further details of the models and dataset are described in:
Yang, Tianzhong, Chong Wu, Peng Wei, and Wei Pan. "Integrating DNA sequencing and transcriptomic data for association analyses of low-frequency variants and lipid traits." Human Molecular Genetics (2020).

Disclaimer: The user assumes the entire risk associated with its use of these data and is responsible to comply with any data usage policy from the original FHS study.

Enjoy!

TZ

2019.7.24
