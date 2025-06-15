# 🧬 Single-Cell Transcriptomic Insights into Immune Aging in Human PBMCs

This dataset was extracted from the supplementary tables of the publication:

> **Title**: Single-cell transcriptomic landscape of human immune aging  
> **Journal**: Cell Research (Nature Publishing Group), 2021  
> **DOI**: [10.1038/s41422-020-00412-6](https://doi.org/10.1038/s41422-020-00412-6)

---

## 📂 Dataset Description

The data was extracted using OCR techniques from PDF tables and saved in `.parquet` format for easy use in data science pipelines. Each row typically represents a gene, cell type, or age group comparison across various immune cell subtypes derived from peripheral blood mononuclear cells (PBMCs).

Format:  
- **File**: `Immune-Aging-transcriptomic .parquet`  
- **Type**: Tabular dataset  
- **Structure**: Varies per table; gene names, expression levels, p-values, fold changes, and metadata columns may be present.

---

## 🔧 Usage Instructions

### Python (with pandas)

```python
import pandas as pd

df = pd.read_parquet("Immune-Aging-transcriptomic .parquet")
print(df.head())
```

### Use in ML pipelines
- Input for aging clock models
- Feature matrix construction for immune cell classification
- Differential gene expression analysis

---

## 💡 Use Cases

- **Aging Biomarker Discovery**: Identify aging-related genes in immune cells.
- **Comparative Aging Studies**: Use alongside other datasets like Tabula Muris Senis or sc-ImmuAging.
- **Model Benchmarking**: Evaluate immune aging clocks using preprocessed features.
- **Longevity Research**: Investigate immune signatures linked to lifespan and healthspan.
- **Multi-omics Integration**: Combine with telomere, methylation, or proteomic datasets.

---

## 📚 Citation

If you use this dataset, please cite the original paper:

> Yang, J., Zheng, Y., Gou, X. et al. Single-cell transcriptomic landscape of human immune aging. *Cell Research* **31**, 1004–1022 (2021).  
> [DOI:10.1038/s41422-020-00412-6](https://doi.org/10.1038/s41422-020-00412-6)

---

## 🙏 Acknowledgments

- Dataset extracted and converted to `.parquet` by **Iris Lee** for use in longevity and immune aging hackathons.
- Original research by Yang et al., published in *Cell Research*, provided foundational insights into immune aging.

---

## 📁 License

Please refer to the license of the original publication. This conversion is provided for **non-commercial research purposes only**.
