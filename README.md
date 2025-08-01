# 🧪 Antimalaria Drug-Likeness Screening with RDKit

This project uses Python and RDKit to analyze the drug-likeness of 23 known antimalarial compounds. The goal is to filter and identify compounds that satisfy **Lipinski’s Rule of Five**, a commonly used rule-of-thumb to evaluate if a compound is likely to be an orally active drug in humans.

---

## 📂 File Included
- `antimalaria.csv`  
  A list of 30 known antimalarial compounds and their SMILES (molecular structure) strings. This is the **raw input** data used for screening.

- `druglikes.csv`  
  The **output** after applying RDKit descriptors and Lipinski’s Rule of Five. It includes:
  - Compound name
  - Molecular weight
  - LogP (hydrophobicity)
  - Number of hydrogen bond donors
  - Number of hydrogen bond acceptors
  - A `DrugLike` flag indicating if the compound passed the filter
---

## 📊 What is Lipinski’s Rule of Five?

A compound is likely to be orally active if it meets these conditions:
- Molecular weight < 500 Da
- LogP < 5
- H-bond donors < 5
- H-bond acceptors < 10

Compounds that meet all four are marked as `DrugLike = True`.

---

## 🧰 Tools Used

- [RDKit](https://www.rdkit.org/) — cheminformatics toolkit for calculating molecular descriptors
- [Pandas](https://pandas.pydata.org/) — for data manipulation
- Google Colab — for running the notebook in the cloud

---

## 🚀 How to Reproduce

1. Open the Jupyter Notebook in Google Colab or locally.
2. Install RDKit:
   ```bash
   pip install rdkit-pypi

## ✍️ Author
Created as a beginner cheminformatics project to explore drug screening techniques and molecular descriptors.
