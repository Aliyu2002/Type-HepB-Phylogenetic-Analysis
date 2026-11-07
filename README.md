# Hepatitis B Virus (HBV) In-Silico Genomic & Phylogenetic Analysis

## Overview
This repository contains an automated bioinformatics pipeline designed to bridge clinical diagnostics with molecular epidemiology. Developed as an independent research extension of undergraduate work on Hepatitis B seroprevalence at Modibbo Adama University and community health outreaches in Sunkani, this project programmatically mines, aligns, and reconstructs the phylogenetic relationships of West African HBV isolates.

## Clinical Significance
While traditional wet-lab serological assays (e.g., HBsAg rapid tests and ELISAs) effectively diagnose current infections, they cannot track viral evolution, mutation drift, or emergence of vaccine-escape variants. By coupling grassroots public health screening data with computational genomics, this pipeline enables researchers to:
1. **Identify Single Nucleotide Polymorphisms (SNPs):** Pinpoint exact base-pair mutations across viral strains.
2. **Track Regional Divergence:** Use distance matrices and Neighbor-Joining algorithms to map how viral lineages circulate within West Africa.
3. **Inform Public Health Strategy:** Provide actionable genomic insights to support vaccination and therapeutic design.

## Pipeline Architecture
The analysis is executed via a Python-based Jupyter Notebook (`HepatitisB_Analysis.ipynb`) utilizing the following computational stack:
- **Data Mining (`Bio.Entrez`):** Programmatically queries the NCBI Nucleotide database to fetch complete viral genomes matching specific geographic and organismal criteria.
- **Sequence Parsing (`Bio.SeqIO`):** Handles FASTA formatting and data manipulation locally.
- **Multiple Sequence Alignment (`MUSCLE`):** Executes high-performance matrix alignment via a local binary engine to stack homologous base pairs across strains.
- **Phylogenetic Reconstruction (`Bio.Phylo` & `Matplotlib`):** Calculates identity distance matrices and constructs Neighbor-Joining evolutionary trees.

## Repository Contents
- `HepatitisB_Analysis.ipynb`: The core interactive Jupyter notebook containing the end-to-end pipeline.
- `HepB_Nigeria_Genomes.fasta`: Raw genomic dataset retrieved from NCBI.
- `HepB_Aligned.fasta`: Mathematically aligned sequence matrix.

## Author
**Aliyu Saad Bose**  
*Assistant Laboratory Technologist | B.Tech Science Laboratory Technology (Microbiology)*  
Focus: Infectious Disease Microbiology, Pathogen Genomics, and Translational Public Health.
