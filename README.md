# Source code for the report on FAPESP process number 2021/10532-6.

The files in this repository contain all of the source code used to complete the study done for the project "Use of Single-Cell RNAseq technology to identify and characterize Plasmodium knowlesi sexual stages". This study aimed to compare three different synchronization methods – MACS, Percoll and saponin – from four different Plasmodium falciparum samples to know which one has the best recuperation ratio.

The files are divided as follow:

1) first_steps - source code in Python to clean and process the initial data.
2) parse_bam - source code in Python to parse through the mapped genes file to determine the number of unique reads in the sample and select those that will be used for biological analyses.
3) count_table - source code in Python to generate and populate a table containing all the cells that are suitable for the analysis and how many times each gene was sequenced for each of those cells.
4) create_pca - source code in R to process the count table and create a PCA (Principal Component Analysis) based on it.
5) annotate_pca - source code in R to annotate the PCA graph using gene expression
6) id_pop - source code in R to identify the population shown on the saponin 1 and Percoll graphs
