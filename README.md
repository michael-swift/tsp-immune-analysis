# TabulaSapiens

this repository contains the code used to analyze the immune compartment of Tabula Sapiens. 

I used a snakemake workflow to assemble BCRs/TCRs and integrate datasets from Smart-Seq2 and 10X genomics. 

Gene Expression data for Tabula Sapiens (h5ad files) was downloaded from the Tabula Sapiens websites.

I mostly make use of scanpy and scirpy, two valuable tools for analyzing single-cell RNA sequencing data.

Note that in most notebooks I specify relative paths to large files not housed in this repository. These files would need to be downloaded and the end user would need to point to the relevant data. 

explanation of directories:

preprocessing/ contains the snakemake workflow I used to integrate the data, including the raw outputs of igblast

metadata/ contains files used in analyses such as dissociation genes or cell cycle genes

data/ contains intermediate and final tables used for analysis

noteboks/ contains the ipython notebooks I used analyze and generate figures from the data
