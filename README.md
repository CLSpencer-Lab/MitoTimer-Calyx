# MitoTimer Aging Analysis

## Project Overview

This repository contains the data analysis workflow, statistical testing, and figure generation for a Drosophila MitoTimer aging study.

MitoTimer is a fluorescent reporter that shifts from green to red as mitochondria redox state fluctuates. This project examines mitochondrial health across age groups and treatment conditions in neuronal and glial populations using the Gal4/UAS system.

Genotypes analyzed:

* nSyb-Gal4/UAS-MitoTimer (neuronal expression)
* Repo-Gal4/UAS-MitoTimer (glial expression)

Experimental groups include:

* Young
* Middle-aged
* Old

Additional analyses compare paraquat-treated and untreated flies.

---

## Experimental Workflow

1. Brains were dissected, immunostained, and imaged using confocal microscopy.
2. Regions of interest (ROIs) were selected in Fiji/ImageJ.
3. Red:green fluorescence ratios and integrated density measurements were collected.
4. Data was imported into R for statistical analysis and visualization.
5. Figures and statistical outputs were generated automatically through the analysis pipeline.

---

## Repository Structure

```text
.
├── data/
├── scripts/
├── figures/
├── results/
└── README.md
```

### data/

Contains raw or processed fluorescence measurements exported from ImageJ.

### scripts/

Contains R scripts and R Markdown files used for data cleaning, statistical analysis, and figure generation.

### figures/

Contains publication-quality figures generated from the analysis pipeline.

### results/

Contains exported statistical outputs including:

* ANOVA tables
* Tukey post hoc comparisons
* Student's t-tests
* Integrated density analyses

---

## Statistical Analysis

Analyses were performed in R using:

* dplyr
* tidyr
* ggplot2
* ggpubr
* rstatix
* readxl
* patchwork
* janitor

Statistical tests include:

* One-way ANOVA
* Tukey's multiple-comparison test
* Student's t-test

Significance thresholds:

* * p < 0.05
* ** p < 0.01
* *** p < 0.001

---

## Generated Outputs

The analysis pipeline generates:

### Figures

* Age-related MitoTimer ratio plots
* Paraquat treatment comparison plots
* Integrated density plots

### Statistical Results

* Age-group ANOVA results
* Tukey post hoc comparisons
* Treatment comparison t-tests
* Integrated density statistical analyses

---

## Author

Abigail Wendland

Cellular Neuroscience, Florida Atlantic University

Wilkes Honors College

