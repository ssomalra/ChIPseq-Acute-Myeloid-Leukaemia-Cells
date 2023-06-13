# ChIP-seq Pipeline 
This repository contains the code and documentation for a ChIP-seq pipeline that I used for training and understanding the ChIP-seq analysis workflow. The pipeline incorporates various tools and steps to process and analyze ChIP-seq data.

## Overview
ChIP-seq (Chromatin Immunoprecipitation Sequencing) is a widely used  technique for studying protein-DNA interactions and identifying locations on the genome that are bound by a protein of interest. This project aims to provide a comprehensive ChIP-seq pipeline that can be used as a reference for understanding the analysis steps involved. The steps and tools involved in this pipeline are described below.

## Pipeline Summary
The following tools were utilized in the ChIP-seq pipeline:
1.  Download the FASTQ files from SRA ([`Fastq-dump`](https://rnnh.github.io/bioinfo-notebook/docs/fastq-dump.html))
2.  Quality Control ([`FastQC`](https://www.bioinformatics.babraham.ac.uk/projects/fastqc/))
3.  Trim Adaptors ([`TrimGalore`](https://github.com/FelixKrueger/TrimGalore/blob/master/Docs/Trim_Galore_User_Guide.md))
4.  Alignment ([`HISAT2`](http://daehwankimlab.github.io/hisat2/manual/))
5.  Binary Index SAM File ([`Samtools`](http://quinlanlab.org/tutorials/samtools/samtools.html))
6.  Peak Calling ([`MACS2 callpeak`](https://hbctraining.github.io/Intro-to-ChIPseq/lessons/05_peak_calling_macs.html))
7.  Call Differential Peaks ([`MACS2 bdgdiff`](https://github.com/macs3-project/MACS/wiki/Call-differential-binding-events))
8.  Annotate Peaks ([`Homer`](http://homer.ucsd.edu/homer/ngs/annotation.html))

Refer to the documentation of each tool for more information on their usage and specific parameters.

## Data Source
The ChIP-seq data used in this project was downloaded from NCBI ([GEO: GSE173995](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE173995)). The dataset consists of ChIP-seq data collected from THP-1 cells, which are human leukemia cells. The following files were downloaded:
- Control Samples: SRR18643804 and SRR14458872
- Treatment Samples: SRR14458865 and SRR14458869

*Note: The provided data serves as an example dataset for training purposes and understanding the pipeline.


