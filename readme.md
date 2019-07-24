In this folder, we present the weights we trained from the Framingham Heart Study (off-spring and third-generation cohorts). The weights are trained from 2,443 samples in total. 

There are three files:
1. CV_full_weights.tar.gz contains weights trained from CVs-only models
2. Joint_full_weights.tar.gz contains weights trained from joint models (CVs and RVs)
3. RV_full_weights.tar.gz contains weights trained from RVs-only models

After unzip the files, there are multiple .RDat files with the name of genes (official symbol). 

In each .RDat file, there are three components:
1. bimfile: contains the SNP location (hg19), reference allele, and alternative allele
2. R2: contains Rsq of cross-validation with lambda.1se and lambda.min and their corresponding number of cis-eQTLs
3. wgt.matrix: contains weights trained with cross-validation for lambda.1se and lambda.min


Further details of the model are described in:
Yang T, Wu C, Wei P, Pan W. Integration of DNA seequencing and transcriptomic data for association analyses of rare variants and lipid traits (unpublished work)

Enjoy!
TZ
