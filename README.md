![nfcore/test-datasets](docs/images/test-datasets_logo.png)

Test data to be used for automated testing with the nf-core pipelines

# Table of Contents

- [Table of Contents](#table-of-contents)
- [Test data for SeqInspector](#test-data-for-seqinspector)
  - [MiSeq](#miseq)
    - [220422\_M11111\_0222\_000000000-K9H97](#220422_m11111_0222_000000000-k9h97)
  - [NovaSeq6000](#novaseq6000)
    - [200624\_A00834\_0183\_BHMTFYDRXX](#200624_a00834_0183_bhmtfydrxx)
  - [PromethION](#promethion)
    - [20230505\_1857\_1B\_PAO99309\_94e07fab](#20230505_1857_1b_pao99309_94e07fab)


# Test data for SeqInspector

This folder contains demultiplexed data generated from the test data for the [demultiplex pipeline](https://github.com/nf-core/test-datasets/tree/demultiplex). Both MiSeq and NovaSeq6000 datasets were demultiplexed using bcl2fastq, and randomly subsampled with `seqtk sample -s100`

## MiSeq
This folder contains input samplesheet and single-end demultiplexed fastq files generated from a MiSeq run.

### 220422_M11111_0222_000000000-K9H97

## NovaSeq6000

This folder contains input samplesheet and single-end demultiplexed fastq files generated from a NovaSeq6000 run.

### 200624_A00834_0183_BHMTFYDRXX

## PromethION

### 20230505_1857_1B_PAO99309_94e07fab
Single-sample run, accessed via `aws s3 ls --no-sign-request s3://ont-open-data/giab_2023.05/flowcells/hg001/20230505_1857_1B_PAO99309_94e07fab/`

Passed and failed `fastq` files were derived from
- `pod5_passed/PAO99309_pass__94e07fab_c3641428_1.pod5` 
- `pod5_fail/PAO99309_fail__94e07fab_c3641428_1.pod5`

Both files were basecalled via `Dorado` (hac), coverted to `fastq` via `samtools` and randomly subsampled with `seqtk sample -s100` to 50 passed and 10 failed reads.

Oxford Nanopore Technologies Benchmark Datasets was accessed on 2024-03-21 from https://registry.opendata.aws/ont-open-data.
