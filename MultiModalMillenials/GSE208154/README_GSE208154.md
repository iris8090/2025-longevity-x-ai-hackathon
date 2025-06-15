# GSE208154 – Complete Cell Atlas of Aging C. elegans

## 📄 Description
This dataset provides a comprehensive single-cell RNA sequencing (scRNA-seq) profile of *C. elegans* across six adult time points. It is a highly curated developmental and aging atlas, useful for longevity, developmental biology, and transcriptomic studies.

## 📊 Dataset Summary
- **Species:** Caenorhabditis elegans
- **Type:** Single-cell RNA-seq (scRNA-seq)
- **Samples:** 11 GSM samples from GEO
- **Format:** 
  - `GSE208154_expression_sparse.parquet`: Sparse gene expression matrix
  - `GSE208154_metadata.parquet`: Cell metadata

## 📁 Files Included
- `GSE208154_expression_sparse.parquet`
- `GSE208154_metadata.parquet`

## 📥 How to Load
```python
import scipy.sparse
import pandas as pd

# Load expression matrix
X = scipy.sparse.load_npz("GSE208154_expression_sparse.parquet")

# Load metadata
metadata = pd.read_parquet("GSE208154_metadata.parquet")
```

## 💡 Use Cases
- Aging research in model organisms
- Cell type classification and developmental biology
- Benchmarking unsupervised and supervised learning on scRNA-seq data
- Pseudotime or trajectory inference studies

## 📚 Citation
If you use this dataset, please cite:
> Lipinszki, Z., et al. (2022). A complete single-cell transcriptomic atlas of aging *C. elegans*. *Nature Aging*, DOI: [10.1038/s43587-022-00217-x](https://doi.org/10.1038/s43587-022-00217-x)

## 🙏 Acknowledgments
We thank Calico Life Sciences for generating and sharing this valuable resource and NCBI GEO for providing public access.

Curated and converted by Iris Lee-participant of the Longevity Hackathon 2025.
