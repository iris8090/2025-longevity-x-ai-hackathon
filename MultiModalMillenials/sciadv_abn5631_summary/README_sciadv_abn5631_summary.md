# sc-ImmuAging – Human PBMC Single Cell Aging Clock Dataset

This repository contains a summary of tables extracted from the supplementary materials of the publication:

> **"A single-cell immune clock of human aging"**  
> *Science Advances, 2022*  
> DOI: [10.1126/sciadv.abn5631](https://doi.org/10.1126/sciadv.abn5631)

The extracted tables are converted into a structured `.parquet` file for easier use in computational pipelines.

---

## 📦 Dataset Description

| Table      | Description                                                             |
|------------|-------------------------------------------------------------------------|
| Table S1   | Summary of scRNA-seq datasets used in this study (public + in-house)   |
| Table S2   | Aging scores and model performance across models and cell types        |
| Table S3   | Gene-level feature importance for predictive aging models              |

These tables provide high-level information to replicate or interpret the immune aging clock models developed using single-cell RNA-seq data from human PBMCs.

---

## 🔧 Usage Instructions

### Load the Parquet File in Python

```python
import pandas as pd

df = pd.read_parquet("sciadv_abn5631_summary.parquet")
print(df)
```

---

## 💡 Use Cases

- Investigating immune cell aging patterns in human PBMCs
- Benchmarking single-cell predictive aging models
- Training or validating ML models using gene-level feature importance
- Augmenting multi-omics longevity studies

---

## 📚 Citation

If you use this dataset, please cite:

> Ma, L., et al. (2022). A single-cell immune clock of human aging. *Science Advances*, 8(46), eabn5631.  
> DOI: [10.1126/sciadv.abn5631](https://doi.org/10.1126/sciadv.abn5631)

---

## 🙏 Acknowledgments

This dataset is derived from the supplementary materials of the original publication.  
Data conversion and formatting by **Iris Lee** for use in longevity-related research and AI health hackathons.