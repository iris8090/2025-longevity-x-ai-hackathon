# 🧬 sc-ImmuAging – Human PBMC Single-Cell Aging Clock Dataset

This dataset includes curated feature selections from peripheral blood mononuclear cells (PBMCs) used to train aging clock models across five major immune cell types. It was derived from the **sc-ImmuAging** project to understand how aging affects the immune system at the single-cell level using machine learning models.

---

## 📦 Dataset Contents

- `sc-ImmuAging.parquet` — Long-format data containing gene features per immune cell type:
  - CD4 T cells
  - CD8 T cells
  - Monocytes
  - NK cells
  - B cells

---

## 💡 Use Cases

- 🧠 **Aging Clock Development**: Train regression models to predict biological age per cell type.
- 🔬 **Immune System Aging Analysis**: Study gene-level contributions to age-related changes across immune subsets.
- 🧬 **Biomarker Discovery**: Identify robust transcriptomic signatures of aging in blood-derived cells.
- 🛠 **Feature Selection Benchmarking**: Compare machine learning models and feature selection strategies in scRNA-seq datasets.
- 📊 **Multi-Omics Integration**: Align transcriptomic aging features with epigenetic clocks or proteomics.

---

## 📖 Citation

If you use this dataset, please cite the original study:

**Dos Santos, Osorio et al. (2022).**  
"A single-cell transcriptomic atlas of the human immune system reveals age-related changes in PBMC composition and function."  
*Science Advances*, 8(45):eabq3784.  
https://doi.org/10.1126/sciadv.abq3784

---

## 🧬 Dataset Description

This dataset was extracted from the **sc-ImmuAging** study that built predictive aging clocks using PBMC single-cell RNA-seq profiles. The features represent selected gene markers associated with aging across five immune cell types. Each list was curated for machine learning model input.

**Original Data Source**:  
[GitHub Repository](https://github.com/dosorio/sc-ImmuAging)  
[Published Paper](https://www.science.org/doi/10.1126/sciadv.abq3784)

---

## 🙏 Acknowledgments

- Original authors of the sc-ImmuAging dataset and publication.
- Curated and converted to `parquet` format by **Iris Lee** for ease of machine learning usage.
- Thanks to the open science community enabling downstream applications of single-cell data.