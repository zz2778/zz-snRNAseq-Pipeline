# zz-snRNAseq-Pipeline: Standardized Single-Nucleus RNA-seq Analysis Framework

A modular, reproducible, and standardized computational pipeline designed for single-nucleus RNA sequencing (snRNA-seq) analysis in neurodegenerative diseases (e.g., Alzheimer's Disease and ALS).

## 🧬 Scientific Motivation
Neurodegenerative diseases involve complex intercellular crosstalk and progressive transcriptomic shifts. This pipeline provides a rigorous computational workflow to uncover cell-type-specific pathology, early cellular stress responses, and lineage trajectory dynamics.

## ⚙️ Standardized Workflow
1. **Quality Control (QC)**: Cell/nucleus filtering, mitochondrial RNA thresholding, and doublet detection.
2. **Normalization & Feature Selection**: Total-count normalization, log-transformation, and HVG selection.
3. **Integration & Batch Correction**: Dimensionality reduction (PCA) and Harmony-based integration to remove experimental batch noise.
4. **Graph Clustering & Cell Annotation**: Leiden community detection paired with canonical biomarker mapping.
5. **Trajectory & Pathway Enrichment**: PAGA lineage inference and GO/KEGG pathway enrichment (GSEAPY).

## 📂 Project Structure
```text
zz-snRNAseq-Pipeline/
├── notebooks/              # Interactive step-by-step tutorials
│   ├── 01_qc_filtering.ipynb
│   ├── 02_normalization_hvg.ipynb
│   ├── 03_integration_harmony.ipynb
│   ├── 04_clustering_annotation.ipynb
│   └── 05_trajectory_enrichment.ipynb
├── src/                    # Encapsulated Python processing scripts
├── results/                # High-resolution figures and output tables
└── README.md               # Documentation
