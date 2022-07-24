# "Foliar fungal communities depend on crop identity and neighboring vegetation in agroecosystems"
### Whitaker, B.K., Heiniger, R., Hawkes, C.V.


This repository includes the R code, data files, small scripts, and a metadata file to supplement the manuscript by Whitaker et al. "Foliar fungal communities depend on crop identity and neighboring vegetation in agroecosystems".

The sample matrix ("XXX.csv") includes information about each sample collected from XXX

The ASV matrix ("XXX.csv") includes the number of amplicon sequence variant (ASV) reads for each sample (rows) and unique ASV (columns). The raw sequence data used to generate this matrix is available through the NCBI SRA database under accession number PRJNA845782 (https://www.ncbi.nlm.nih.gov/bioproject/PRJNA845782/).

The taxonomy matrix ("XXX.csv") includes the taxonomic classification of each unique ASV as was used in the manuscript.

Detailed information about column headers in the sample matrix and taxonomy matrix can be found in the metadata file "XXXX.xlsx".

The XXXX Rmd documents provide the pipeline for bioinformatic analysis using DADA2, taxonomic classification of fungal ASVs and removal of plant ASVs, and the analysis of the fungal community as it appears in the paper. They should be run in this order: DADA2_pipeline.Rmd > TaxonomicClassification.Rmd > CommunityAnalyses.Rmd

The /code folder contains the batch and R scripts necessary to run XXX. Data necessary to run the analyses can be found in /data folder.

Please see the manuscript for details and full reference information.
