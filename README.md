# CUT&RUN Shell Pipeline

This repository provides a universal, SLURM-compatible shell script for processing CUT&RUN sequencing data in mouse (mm10).

---

## 🔧 Features

- Adapter trimming with `fastp`
- Alignment with `bowtie2`
- Filtering, sorting, and indexing with `samtools`
- Duplicate removal using `Picard`
- Coverage track generation with `deepTools` (`bamCoverage`)

---

## 🚀 Quick Start

Edit these variables at the top of the script:

```bash
input_dir="/path/to/fastq"
output_dir="/path/to/output"
bowtie2_index="/path/to/mm10/bowtie2/index/genome"
picard_jar="/path/to/picard.jar"
