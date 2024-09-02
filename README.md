# LongMod123

The development of long-read sequencing technologies has introduced a powerful new tool to the field of epigenetics by enabling the direct detection of DNA modifications, such as DNA methylation, at single-base resolution. This produces novel opportunities for studying the role of DNA methylation in gene regulation, imprinting, and disease. Analysis of the data produced by long-read sequencing technologies requires the development of new software tools to handle the unique characteristics of the data, such as the modBAM format in which the data is output, and the length of the sequenced reads. The `NanoMethViz` package provides a suite of tools for loading in this methylation data, visualising regional and genome-wide methylation patterns, and exporting data for identifying differentially methylated regions (DMRs) using other Bioconductor software such as `bsseq`, `DSS`, `dmrseq` and `edgeR`. In this workflow article, we demonstrate how to use the `NanoMethViz` package and other Bioconductor software to perform a complete analysis of long-read 5mC DNA methylation data starting from the raw data, to exploratory analysis, DMR identification, and visualisation of the results.

# Installation

This package contains all the dependencies required to run the workflow. To install the package, run the following command:

```r
BiocManager::install("mritchielab/LongMod123", dependencies = TRUE)
```

Then follow the workflow from https://mritchielab.github.io/LongMod123/articles/workflow.html

## Docker

A docker image with the data and required packages can be obtained by running

```bash
docker pull ghcr.io/mritchielab/longmod123:latest
```
