
# 🧬 Smulders Longevity Extracted Dataset

This dataset was extracted from the publication:

> **Genetics of human longevity: From variants to genes to pathways**  
> *Journal of Internal Medicine, 2023 — Smulders et al.*  
> DOI: [10.1111/joim.13690](https://doi.org/10.1111/joim.13690)

It contains structured gene names and SNP identifiers mentioned throughout the paper.

---

## 📄 Dataset Description

| Column | Description                  |
|--------|------------------------------|
| type   | Entry type: `Gene` or `SNP`  |
| id     | The gene name or SNP ID      |

The gene names are uppercase identifiers, and SNPs follow the common `rs` format (e.g., rs429358).

---

## 🔧 Usage Instructions

### Load in Python

```python
import pandas as pd

df = pd.read_parquet("smulders_longevity_extracted.parquet")
print(df.head())
```

---

## 🚀 Use Cases

- Gene prioritization for longevity research
- Mapping SNPs from literature to existing aging gene databases
- Input for polygenic risk score (PRS) modeling
- Enhancing datasets like LongevityMap with literature-derived signals

---

## 📚 Citation

If you use this dataset, please cite the original paper:

> Smulders, Y. M., et al. (2023). Genetics of human longevity: From variants to genes to pathways. *Journal of Internal Medicine*.  
> [https://doi.org/10.1111/joim.13690](https://doi.org/10.1111/joim.13690)

---

## 🙏 Acknowledgments

Extracted and compiled by Iris Lee for longevity research and hackathon use.
