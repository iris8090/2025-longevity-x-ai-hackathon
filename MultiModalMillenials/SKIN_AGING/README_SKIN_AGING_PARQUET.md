# A Single-Cell Transcriptomic Atlas of Human Skin Aging

This dataset contains structured tables extracted from the supplementary materials of the publication:

> **"A single-cell transcriptomic atlas of human skin aging"**  
> *Cell Reports, 2020*  
> DOI: [10.1016/j.celrep.2020.108132](https://doi.org/10.1016/j.celrep.2020.108132)

The data has been processed from the publication PDF into a `.parquet` file to facilitate downstream analysis and integration into machine learning workflows.

---

## 📦 Dataset Description

The dataset includes multiple tables capturing aging-related transcriptomic changes in human skin tissue at the single-cell level. Tables were extracted using PDF parsing tools and contain gene expression summaries and annotations useful for skin biology and aging research.

---

## 🔧 Usage Instructions

To load the Parquet file in Python:

```python
import pandas as pd

df = pd.read_parquet("skin_aging_data.parquet")
print(df.head())
```

---

## 🚀 Use Cases

- Aging biomarker discovery in dermal and epidermal compartments
- Training skin-specific biological age predictors
- Integrating skin aging profiles with other tissue atlases
- Cross-species comparison of skin aging signatures
- Evaluation of anti-aging interventions at single-cell resolution

---

## 📖 Citation

If you use this dataset, please cite:

**Xie, W., et al.** *A single-cell transcriptomic atlas of human skin aging*. Cell Reports, 2020.  
DOI: [10.1016/j.celrep.2020.108132](https://doi.org/10.1016/j.celrep.2020.108132)

---

## 🙏 Acknowledgments

This dataset was curated and converted by **Iris Lee** for open access machine learning research in aging biology and skin regeneration.

Source publication by Xie et al. (2020) — Cell Reports.
