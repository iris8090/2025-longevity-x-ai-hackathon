# GSE167186 – Single-Nucleus RNA-Seq of Aged Human Skeletal Muscle

**Organism**: *Homo sapiens*  
**Tissue**: Human skeletal muscle  
**Samples**: 23 individuals (young and aged)  
**Technique**: 10x Genomics single-nucleus RNA-seq  
**Data Type**: Processed sparse expression matrix and cell metadata  

---

## 🧭 Description

This dataset contains single-nucleus transcriptomes from human skeletal muscle samples spanning young and aged adult individuals. The goal was to understand the molecular changes in muscle cells associated with aging.

Each sample is represented by a `.h5` file in the original dataset, which we have converted into a unified sparse expression matrix and metadata file for easy access and analysis.

---

## 📂 Files Included

- `GSE167186_expression_sparse.parquet`  
   → Gene expression matrix (sparse, cells × genes), saved using `scipy.sparse.save_npz`

- `GSE167186_metadata.parquet`  
   → Cell-level metadata, including sample ID and batch assignment

---

## 📥 How to Use

```python
import pandas as pd
from scipy import sparse

# Load expression matrix
X = sparse.load_npz("GSE167186_expression_sparse.parquet")

# Load metadata
meta = pd.read_parquet("GSE167186_metadata.parquet")
```

---

## 💡 Use Cases

- Investigating age-related changes in skeletal muscle at single-cell resolution
- Benchmarking trajectory inference or cell clustering tools
- Identifying differentially expressed genes between young and aged muscle
- Studying cell-type-specific transcriptional signatures of human aging

---

## 🔗 Citation

If you use this dataset, please cite:

> Rubenstein et al. (2022). "Single-nucleus transcriptomics of human skeletal muscle reveals molecular signatures of aging." *Nature Aging*. DOI: [10.1038/s43587-022-00221-1](https://doi.org/10.1038/s43587-022-00221-1)

---

## 🙏 Acknowledgments

Original dataset from GEO Accession [GSE167186](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE167186).  
Data curated and converted by Iris Lee as part of the 2025 Longevity x AI Hackathon.