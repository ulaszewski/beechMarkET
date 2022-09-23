# beechMarkET - Beech Marker Extraction Tool 
===

**beechMarkET** is a command-line wraper designed for extracting high quality SNPs from the common beech (_Fagus sylvatica_ L.) genome. 

===

# Installation

## **Pre-requisites** - the programs

**Option #1** (recommended)

If you use [conda](https://conda.io/projects/conda/en/latest/user-guide/install/index.html) you can install **beechMarkET** pre-requisited programs by running the following commands in your terminal:
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


**Option #3**

Dokcer image (in preparation)

## **Pre-requisites** - the reference genome

Download the  reference genome of _Fagus sylvatica_ from the [Thines Lab site](http://thines-lab.senckenberg.de/beechgenome/data.html) or from [NCBI Genome repository](https://www.ncbi.nlm.nih.gov/data-hub/genome/GCA_907173295.1/). If needed unzip the assembly and index it with the following command:
```
bwa index -a is **your_reference_name.fasta**
```

## Main wraper install

Download the wraper from this repository by:
```
git clone https://github.com/ulaszewski/beechMarkET.git
```
and
```
cd beechMarkET
chmod +x beechmarket
```

# Running the pipeline
Follow the installation instructions, run the script as shown below and answer the prompt questions
```
./beechmarket
```
