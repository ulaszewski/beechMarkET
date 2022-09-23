# beechMarkET - Beech Marker Extraction Tool 
===

**beechMarkET** is a pipeline designed for extracting high quality SNPs from the common beech (_Fagus sylvatica_ L.) genome. 

===

# Installation

## Conda-based installation (recommended)

If you use conda you can install **beechMarkET** by running the following commands in your terminal:
```
conda config --add channels bioconda
conda create --name beechmarket
conda activate beechmarket
conda install -c bioconda trimmomatic samtools bcftools=1.15.1 bwa
```

## Installation without conda 

Pre-requisites
trimmomatic
bwa
samtools
bcftools (>1.11)
