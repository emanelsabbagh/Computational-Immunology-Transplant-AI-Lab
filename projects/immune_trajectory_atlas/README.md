# Immune Trajectory Atlas After Pediatric Hematopoietic Cell Transplantation

This is the flagship scientific project of the Computational Immunology and Transplant AI Lab (CITA Lab).

The goal of this project is to build the first openly reproducible, multi-dataset 
**immune trajectory atlas** describing how T, B, NK, and myeloid cells recover 
after pediatric hematopoietic cell transplantation (HCT), using public data as 
a foundation.

---

## 🔬 Scientific Motivation

Immune recovery after transplant determines:
- infection risk  
- relapse risk  
- GVHD risk  
- survival outcomes  

Yet the field still lacks a **standardized, data-driven map** of immune trajectories 
after HCT in children.

This project aims to address that gap.

---

## 🧪 Data Sources (Public)

We will begin with public datasets:

- **scRNA-seq PBMC datasets** (10x PBMC3k, HCA, GEO pediatric HCT datasets)
- **ImmPort** immune phenotyping datasets
- **FlowRepository** cytometry panels
- **TCR repertoire data** from iReceptor (optional, phase 2)

No protected or institutional datasets will be used in this public version.

---

## 🧠 Planned Analyses

### Phase 1 — scRNA-seq Baseline
- Load and process PBMC public datasets  
- Quality control (QC)  
- Normalization  
- PCA, UMAP, clustering  
- Cell type annotation (T, B, NK, mono, dendritic)  

### Phase 2 — Trajectory Building
- Pseudotime analysis (Scanpy DPT, Palantir, Slingshot)  
- Early → mid → late immune states  
- Identify exhausted/hyperactive/inhibited states  

### Phase 3 — Immune Curve Extraction
- Extract T, B, NK, mono cell proportions across timepoints  
- Fit splines / GAM curves  
- Compare trajectories across:
  - disease types  
  - conditioning regimens  
  - donor types  

### Phase 4 — Visualization & Interpretation
- Heatmaps of gene programs  
- Trajectory plots  
- Cell-cell communication maps (optional)  

---

## 📦 Expected Outputs (for publication)

- A reproducible pipeline for immune trajectory modeling  
- A visual “atlas” of immune recovery states  
- A preprint or manuscript draft  
- Code notebooks (public and documented)  

This project will anchor CITA Lab’s identity and demonstrate its scientific value.

---

## 📁 File Structure (planned)

- `01_data/` — public dataset links or loaders  
- `02_notebooks/` — QC, clustering, annotation  
- `03_trajectories/` — pseudotime analyses  
- `04_results/` — figures, summaries  
- `05_manuscript/` — draft/notes when ready  

---

## 👩‍🔬 Lead Scientist

** Eman Elsabbagh, MD, MSc **  
Computational Immunology and Transplant AI Lab (CITA Lab)

---

## 🔒 Ethics and Data Use

This project uses only **public datasets** and contains **no PHI**.  
Future IRB-based expansions will occur within the appropriate institutional framework.
