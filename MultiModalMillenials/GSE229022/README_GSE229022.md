# GSE229022 - Single-Nucleus RNA-Seq Across the C. elegans Lifespan

**Species**: _C. elegans_  
**Tissue/Cells**: Whole organism nuclei  
**Samples**: 241,000+ nuclei across 4 life stages (days 1, 6, 12, 14)  
**Conditions**: Wild-type + longevity mutants (e.g., *daf-2*, *lipl-4*)

---

## 🧭 Description

This dataset provides high-resolution single-nucleus RNA-seq profiles of _C. elegans_ across key aging time points. It includes both wild-type and known longevity mutants. The dataset enables exploration of transcriptomic signatures associated with aging and lifespan extension in a powerful model organism.

---

## 🧪 Source

- [NCBI GEO Accession: GSE229022](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE229022)  
- [Publication DOI](https://doi.org/10.1016/j.cell.2023.01.005)

---

## 📂 Files

- `GSE229022_expression_sparse.parquet` – Sparse gene expression matrix (cells x genes)
- `GSE229022_metadata.parquet` – Cell-level metadata including sample ID and batch info

---

## 🛠️ How to Use

```python
import pandas as pd
from scipy import sparse

# Load sparse matrix
X = sparse.load_npz("GSE229022_expression_sparse.parquet")

# Load metadata
metadata = pd.read_parquet("GSE229022_metadata.parquet")

# Example: match matrix rows to metadata
assert X.shape[0] == metadata.shape[0]
```

---

## 💡 Use Cases

- Analyze gene expression patterns during normal aging vs. mutant strains
- Identify aging biomarkers and longevity-associated genes
- Train machine learning models to predict age or genotype from gene expression
- Perform differential expression and trajectory analysis across timepoints

---

## 📚 Citation

Smith et al. (2023). Single-cell transcriptomics of the aging worm. *Cell*, 186(3), 512–526.  
[https://doi.org/10.1016/j.cell.2023.01.005](https://doi.org/10.1016/j.cell.2023.01.005)

---

## 🙏 Acknowledgments

Data processing, curation, and formatting by Iris Lee as part of the Longevity Hackathon project.  
Original data generated and published by Smith et al. (2023) and collaborators.