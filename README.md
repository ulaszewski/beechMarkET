# beechMarkET - Beech Marker Extraction Tool 
===

**beechMarkET** is a command-line wraper designed for extracting high quality SNPs from the common beech (_Fagus sylvatica_ L.) genome. 

===

# Installation

## **Pre-requisites** - the programs

**Option #1** (recommended)

If you use [conda](https://conda.io/projects/conda/en/latest/user-guide/install/index.html) you can install **beechMarkET** pre-requisites by running the following commands in your terminal:
```
conda config --add channels bioconda
conda create --name beechmarket
conda activate beechmarket
conda install -c bioconda trimmomatic samtools bcftools=1.15.1 bwa
```

**Option #2**
You can also use independatly install the following programs:

[trimmomatic](https://github.com/usadellab/Trimmomatic)

[bwa](https://github.com/lh3/bwa)

[samtools](https://github.com/samtools/samtools)

[bcftools (>1.11)](https://github.com/samtools/bcftools)

## **Pre-requisites** - the reference genome

Download the  reference genome of _Fagus sylvatica_ from the [Thines Lab site](http://thines-lab.senckenberg.de/beechgenome/data.html) or from [NCBI Genome repository](https://www.ncbi.nlm.nih.gov/data-hub/genome/GCA_907173295.1/). If needed unzip the assembly and index it with the following command:
```
bwa index -a is **your_reference.name.fasta**
```


## Main wraper install

Step 1: Download the compressed and indexed reference genome of _Fagus sylvatica_ from here:
Step 2: Uncompress the refrerence
```
tar xvzf reference.tar.gz
```
Step 2: Download the wraper from this repository
Step 3: Change the mode of the program
```
chmod +x beechmarket
```
