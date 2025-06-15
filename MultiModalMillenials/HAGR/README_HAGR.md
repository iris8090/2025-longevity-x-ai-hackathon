
# 🧬 Human Ageing Genomic Resources (HAGR)

This dataset collection is derived from the Human Ageing Genomic Resources (HAGR), a curated set of databases focusing on the genetics of human aging, longevity, and cellular senescence. It includes several valuable resources formatted as `.parquet` files for easy use in data science and machine learning pipelines.

---

## 📦 Files Included

- `drugage.parquet`: Database of drugs that affect lifespan in model organisms.
- `genage_human.parquet`: Genes associated with aging in humans.
- `genage_models.parquet`: Aging-related genes in model organisms.
- `longevity.parquet`: Genetic variants linked to human longevity.
- `cellage3.parquet`: Genes associated with cellular senescence.
- `signatures1.parquet`: Transcriptional signatures related to age-associated biological pathways.

---

## 🔧 Usage Instructions

```python
import pandas as pd

# Example: Load DrugAge
df = pd.read_parquet("drugage.parquet")
print(df.head())
```

You can load all other `.parquet` files in the same way.

---

## 🔬 Use Cases

- Build predictive models of aging or lifespan using genetic or pharmacological features.
- Identify potential gene-drug-longevity interactions.
- Benchmark aging clocks against curated biological evidence.
- Perform feature importance analysis on senescence-related targets.
- Develop explainable AI models for aging biology.

---

## 📚 Citation

Please cite the original HAGR resource:

> de Magalhães, J. P., et al. (2009). The Human Ageing Genomic Resources: new tools for ageing research. *Nucleic Acids Research*, 37(Database issue), D756–D759.  
> DOI: [10.1093/nar/gkn777](https://doi.org/10.1093/nar/gkn777)

Official site: https://genomics.senescence.info

---

## 🙏 Acknowledgments

Data curated and maintained by the Human Ageing Genomic Resources project.  
Formatting and conversion to `.parquet` for ML use by [Iris Lee](https://huggingface.co/IrisLee).

---

## 🗂️ License

Please review individual dataset licenses on [https://genomics.senescence.info](https://genomics.senescence.info). Most data is freely available for academic and non-commercial use.
