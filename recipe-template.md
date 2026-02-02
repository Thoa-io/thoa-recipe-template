---
# Welcome to the THOA Recipe Template!
# This file is a starting point for creating a new THOA recipe.
#
# This template defines the standard structure for all THOA recipes.
# Please complete each section with your workflow-specific content.
#
# - Title
# - Introduction:
#   What is this recipe about?
#   Why is it important?
#   What kind of data does it use?
#   What kind of methods does it apply?
#   Who is this recipe for?
#
# - Input Data Overview:
#   Description, figure, or general overview of the input data.
#
# - Tutorial Section:
#   Code snippets and THOA commands to run the analysis.
#
# - Result Data Overview:
#   Description of the output data and an overview of the results.
#
# - Final Analysis / Results / Interpretation:
#   Explain what the results mean and how they should be interpreted.

title: recipe Template
description: A starter template for creating new THOA recipes.
image: /recipe-images/template.jpg

# Please start by filling out the title and description
# and by adding a representative image.
#
# Thank you for contributing to the THOA cookbook.
---

## Introduction

This recipe provides a standardized and reproducible workflow to analyze high-throughput biological data and transform raw files into interpretable results.

It is designed to answer questions such as:

* What biological changes are present between samples or conditions?
* Which features (genes, variants, regions) are significantly affected?

### Data

Describe the input data (e.g., bulk RNA-seq, WGS, scRNA-seq) and starting format (e.g., FASTQ, count matrices).

### Methods & Tools

Briefly describe the main processing steps and tools used (e.g., QC, alignment, quantification, statistics, Nextflow, nf-core).

### Target Audience

State who this recipe is for (e.g., bioinformaticians, lab scientists, data analysts) and the required skill level.

### Purpose

Explain why this recipe is useful (e.g., reproducibility, automation, standardized analysis).

---

## Input Data Overview

Briefly describe the structure and type of input data required for this recipe.

### Required Files

- **Raw reads** (`.fastq.gz`)  
  Primary sequencing reads  

- **Sample metadata** (`.csv`)  
  Sample IDs and experimental conditions  

- **Reference genome** (`.fa`)  
  Genome sequence for alignment  

- **Gene annotation** (`.gtf`)  
  Gene models for quantification  



### Input Directory Structure (optional)

```txt
project/
  data/
    sample1_R1.fastq.gz
    sample1_R2.fastq.gz
  metadata/
    samples.csv
  reference/
    genome.fa
    genes.gtf
```

(Optional) Input figure or screenshot showing the data layout.

---

## Tutorial

Step-by-step guide to run the recipe.

### 1. Prepare the Environment

Describe how to access the platform, workspace, or compute environment  
(e.g., login, project setup, permissions).

---

### 2. Configure Parameters (optional)

Describe which parameters must be defined and where they are configured  
(e.g., config file, UI form, environment variables).

```text
<parameter_name>: <value>
<parameter_name>: <value>
````

---

### 3. Run the Workflow

Describe how the workflow is started
(e.g., command-line, web interface, job submission button).

```text
<command or action to start the workflow>
```

---

### 4. Monitor & Troubleshoot

Explain how users can:

* Track job status
* Access logs and reports
* Resume or restart failed runs

```
---

## Result Data Overview

Explain what the outputs are and how to find them.

### Key Outputs

| Output    | Location                      | Description     |
| --------- | ----------------------------- | --------------- |
| Report    | `results/multiqc_report.html` | QC summary      |
| Counts    | `results/counts.tsv`          | Raw gene counts |
| BAM files | `results/bams/`               | Aligned reads   |

### Output Tree (optional)

```txt
results/
  bams/
  counts.tsv
  multiqc_report.html
```

Example Figure

---

## Final Analysis & Interpretation

Describe what users should look for in the results.

* What does a successful run look like?
* How should users interpret findings?
* Common next steps (e.g., DEG analysis, enrichment)

---

## References & Resources

* Pipeline documentation
* Relevant paper or method
* THOA support: [hello@thoa.io](mailto:hello@thoa.io)
