In this folder, we present the weights trained from the Framingham Heart Study (off-spring and third-generation cohorts) with a total sample size of 2,441. 

There are a few files with their name begin with:
1. CV_full_weights.tar.gz contains weights trained from CVs-only models
2. Joint_full_weights.tar.gz contains weights trained from joint models (CVs and RVs)
3. RV_full_weights.tar.gz contains weights trained from RVs-only models

After unzip the files, there are multiple .RDat files with the name of genes (official symbol). 

In each .RDat file, there are three components:
1. bimfile: contains the SNP location (hg19), reference allele, and alternative allele
2. R2: contains Rsq based on elastic net models cross-validated with lambda.1se and lambda.min and their corresponding number of cis-eQTLs
3. wgt.matrix: contains weights trained by elastic net regession cross-validated with lambda.1se and lambda.min

For Joint_full_weights files, we further indicate whether a included SNP is a RV and how many RVs are selected in the final model in R2 (nRV_min) and wgt.matrix (rare_ind), respectively


Further details of the models and dataset are described in:
Yang T, Wu C, Wei P, Pan W. Integration of DNA seequencing and transcriptomic data for association analyses of rare variants and lipid traits (unpublished work)

Enjoy!

TZ

2019.7.24
