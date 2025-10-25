# RNA-seq-Analysis-of-Surface-vs-Cavefish-Brains

**Author:** Lawal Agboola  
**Date:** September 2024  

## Overview
This repository contains a full RNA-seq analysis workflow comparing gene expression between surface and cavefish (Astyanax mexicanus) brains across age groups (young vs old). The analysis aims to uncover molecular mechanisms linked to biological resilience and neurodegeneration resistance in cavefish.

## Analysis Workflow

1. **Load libraries and datasets**  
   Import raw counts and annotation files.

2. **Data preprocessing and normalization**  
   Create a DESeq2 dataset and perform variance-stabilizing transformation (VST).

3. **Exploratory analysis**  
   - PCA visualization of sample clustering.

4. **Differential expression analysis (DESeq2)**  
   - Compare young vs old surface fish brains.  
   - Identify significantly up/downregulated genes.

5. **Gene annotation and filtering**  
   - Merge DEGs with *Astyanax mexicanus* gene names.  
   - Filter by adjusted p-value (≤ 0.05) and |log2FC| ≥ 1.

6. **Functional enrichment (GO & KEGG)**  
   - Map genes to zebrafish orthologs (*Danio rerio*).  
   - Visualize enriched biological processes and pathways.

---

## Outputs
| File | Description |
|------|--------------|
| `GO_Enrichment_SOSY_up.png` | Top GO terms enriched in upregulated genes |
| `KEGG_pathway_enrichment_SOSY_up.png` | KEGG pathways enriched in upregulated genes |
| `up_surface_old_young.csv` | List of upregulated genes (old vs young) |
| `down_surface_old_young.csv` | List of downregulated genes (old vs young) |

---

## Biological Significance
This analysis explores molecular signatures of aging and neurodegenerative resilience in cavefish. Comparing surface and cave populations helps identify protective mechanisms against oxidative stress and neuronal damage.
