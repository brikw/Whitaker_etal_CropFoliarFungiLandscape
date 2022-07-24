# "Foliar fungal communities depend on crop identity and neighboring vegetation in agroecosystems"
### Whitaker, B.K., Heiniger, R., Hawkes, C.V.


This repository includes the R code, data files, small scripts, and a metadata file to supplement the manuscript by Whitaker et al. "Foliar fungal communities depend on crop identity and neighboring vegetation in agroecosystems".

The sample matrix ("MBLand_SbyE_2021-10-04-2nd.csv") includes information about each sample collected from across NC crops in 2019. 4 leaf samples were collected and bulked per plot, with 12 plots per site: from Winter Wheat (WHT, Triticum aestivum), Corn (CRN, Zea mays), Soy (SOY, Glycine max), and Switchgrass (SWCH, Pavi, Panicum virgatum). Leaves collected for Illumina were Flag for WHT and SWCH, Ear leaf for CRN, and 3rd/4th fully-expanded-upper-canopy leaves for SOY. All samples are associated with basic plant size metrics and a measurement for soil moisture. A total of 239 samples were prepped for Illumina sequencing (1 CRN ear plot died before sampling), 60 plants per species/leaf type. An additional 4 samples represent controls of various sorts. A PNA designed by B. Whitaker was used to reduce plant amplification for the SWCH samples. A single MiSeq sequencing was used for all the samples.

The ASV matrix ("MBLand_SbyS.csv") includes the number of amplicon sequence variant (ASV) reads for each sample (rows) and unique ASV (columns). The raw sequence data used to generate this matrix is available through the NCBI SRA database under accession number PRJNA845782 (https://www.ncbi.nlm.nih.gov/bioproject/PRJNA845782/).

The taxonomy matrix ("MBLand_RDP_WarcupDefault_AddUNITE.csv") includes the taxonomic classification of each unique ASV.

Detailed information about column headers in the sample matrix and taxonomy matrix can be found in the metadata file "MBLand_Meta.xlsx".

The DADA2_pipeline.Rmd document performs bioinformatic analysis using DADA2; Taxonomy_Curation.Rmd does taxonomic classification of fungal ASVs and removal of plant ASVs; Structure_Richness_RRPP.Rmd the Structure and Richness (Hyp1) analysis of the fungal communities; CCA_LandscapeBwSites.Rmd contains the CCA and between site dissimilarity landscape model; and LandscapeWithinSites.Rmd contains the models and figures for within site richness and dissimilarity landscape models. They should be run in this order: DADA2_pipeline.Rmd > Taxonomy_Curation.Rmd > Structure_Richness_RRPP.Rmd > CCA_LandscapeBwSites.Rmd > LandscapeWithinSites.Rmd.

The /code folder contains the batch and R scripts necessary to run small codes inside R and the Goolge Earth Engine code. Data necessary to run the analyses can be found in /data folder.

Please see the manuscript for details and full reference information.
