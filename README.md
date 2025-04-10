# Snakemake workflow: `MycoFlow`

[![Snakemake](https://img.shields.io/badge/snakemake-≥6.3.0-brightgreen.svg)](https://snakemake.github.io)
[![GitHub actions status](https://github.com/Kratzcomycete/Fungal-Genome-Processing-Snakemake/workflows/Tests/badge.svg?branch=main)](https://github.com/Kratzcomycete/Fungal-Genome-Processing-Snakemake/actions?query=branch%3Amain+workflow%3ATests)


A Snakemake workflow for processing fungal genome sequencing data. It automates quality control, read trimming, genome assembly, and read mapping, providing a reproducible workflow for fungal genomic analysis.
## Input
Please add the genomes you wish to process into a folder called "raw_reads" (this can be changed by modifying the input parameter for fastp and fastq in the "config.yaml" file).
### They must match the naming convention: {sample}_R1.fastq.gz or {sample}_R2.fastq.gz

## Usage

1. Clone the repository using
```bash
   git pull https://github.com/Kratzcomycete/Fungal-Genome-Processing-Snakemake.git
```
2. Enter the cloned directory
  ```bash
   cd Fungal-Genome-Processing-Snakemake
```
3. Create a conda environment named Fungal-Genome-Processing-Snakemake to run the pipeline inside of
 ```bash
   conda env create --file workflow/envs/environment.yaml
```
4. Activate conda environment before running pipeline
 ```bash
   conda activate Fungal-Genome-Processing-Snakemake
```
5. Run the pipeline using
   ```bash
   snakemake --cores <number_of_cores> --use-conda
   ```

Modifications can be made to the .yaml file for computational adjustments














The usage of this workflow is described in the [Snakemake Workflow Catalog](https://snakemake.github.io/snakemake-workflow-catalog/?usage=<Kratzcomycete>%2F<Fungal-Genome-Processing-Snakemake>).

If you use this workflow in a paper, don't forget to give credits to the authors by citing the URL of this (original) <repo>sitory and its DOI (see above).


* The workflow will occur in the snakemake-workflow-catalog once it has been made public. Then the link under "Usage" will point to the usage instructions if `<owner>` and `<repo>` were correctly set.

This is a test from rstudio
