# Telomere Length and Structure Dataset (PDF Extracted)

This dataset contains structured tables extracted from two peer-reviewed publications focused on telomere sequencing, length measurement, and structure—key biomarkers in aging and age-related disease.

## Dataset Description

The dataset is compiled from:
1. `s41467-024-49007-4.pdf` (Nature Communications)
2. `eScholarship UC item 0t23r589.pdf`

Extracted tables cover:
- Telomere length metrics
- Nanopore sequencing measurements
- Biological age associations
- Sample-level telomere profiles

The final dataset is saved in the file: `telomere_datasets_combined.parquet`

## Usage Instructions

```python
import pandas as pd

df = pd.read_parquet("telomere_datasets_combined.parquet")
print(df.head())
```

## Use Cases

- Train biological aging clocks using telomere length features
- Identify age-related trends in telomere attrition
- Benchmark telomere shortening in disease vs. healthy cohorts
- Integrate into multi-omics aging models

## Citation

If you use this dataset, please cite the original studies:
- [Nature Communications article](https://doi.org/10.1038/s41467-024-49007-4)
- [eScholarship publication](https://escholarship.org/uc/item/0t23r589)

## Acknowledgments

This dataset was curated and processed by **Iris Lee**. Tables were extracted using `pdfplumber` and converted to `.parquet` using `pandas`.

We acknowledge the original authors for the data published in open-access journals.

---

For questions, contact Iris or visit the Hugging Face dataset page.