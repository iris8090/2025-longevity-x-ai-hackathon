# 🧬 Tabula Muris Senis – 10x Dataset (Mouse Aging Atlas)

**Organism**: *Mus musculus*  
**Assay**: 10x Genomics Single Cell 3' v2  
**Tissues**: 16 mouse tissues (e.g., heart, lung, kidney, liver)  
**Cells**: 245,000+ single cells  
**Age groups**: Spanning mouse lifespan (young to old)

---

## 📖 Dataset Description

This dataset is a subset of the Tabula Muris Senis project, a collaborative effort to create a comprehensive single-cell transcriptomic atlas of aging in the mouse. The 10x portion of the data includes over 245,000 cells across 16 tissues profiled using droplet-based 10x Genomics technology. It provides a powerful resource for understanding how aging affects individual cell types across diverse tissues.

---

## 📂 Files Included

- `TMS_expression_sparse.parquet` – Chunked gene expression matrix (cells × genes)  
- `TMS_metadata.parquet` – Metadata per cell (tissue, age, sex, cell type, etc.)

---

## 🚀 Usage Instructions

```python
import pandas as pd

# Load the expression and metadata files
expression = pd.read_parquet("TMS_expression_sparse.parquet")
metadata = pd.read_parquet("TMS_metadata.parquet")

# Optionally merge for analysis
df = expression.join(metadata)
```

Alternatively, load from Hugging Face:

```python
from datasets import load_dataset

ds = load_dataset("longevity-db/tabula-muris-senis-10x")
df = ds["train"].to_pandas()
```

---

## 💡 Use Cases

- **Transcriptomic Aging Analysis**: Discover how aging influences gene expression across cell types and tissues.
- **Cross-Tissue Comparisons**: Study systemic versus tissue-specific aging trajectories.
- **Biological Age Modeling**: Train machine learning models to predict biological age from transcriptomic signatures.
- **Single-Cell Method Development**: Benchmark algorithms for clustering, integration, or trajectory inference on aging data.
- **Sex-Specific Aging Research**: Explore differences in aging across male and female samples.
- **Cross-Species Comparisons**: Integrate this dataset with human aging data to identify conserved mechanisms.

---

## 📚 Citation

If you use this dataset, please cite the original publication:

> **Tabula Muris Consortium** (2020).  
> *A single-cell transcriptomic atlas characterizes ageing tissues in the mouse.*  
> Nature, 583, 590–595.  
> https://doi.org/10.1038/s41586-020-2496-1

---

## 🙏 Acknowledgments

This dataset was produced by the [Tabula Muris Consortium](https://tabula-muris-senis.ds.czbiohub.org/), made possible by the **Chan Zuckerberg Biohub** and the **CZI Initiative**.  
The data was accessed via [cellxgene.cziscience.com](https://cellxgene.cziscience.com) and reformatted by **Iris Lee** for easier community use.

We acknowledge the developers of open-source tools such as `scanpy`, `anndata`, `pandas`, and `pyarrow` that made processing and sharing this dataset possible.

---
