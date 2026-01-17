# Drug-Likeness Filtering and Diversity Selection

This project demonstrates how to use **RDKit** to analyze chemical datasets for drug discovery. The workflow includes:

1. **Drug-likeness filtering**  
   - Applying Lipinski's rule of five to a dataset of SMILES.
   - Minimising the number of violations to select potential drug-like compounds.

2. **Similarity calculation**  
   - Using Tanimoto similarity to compare compounds to a reference molecule (e.g., Doxorubicin).  
   - Filtering compounds with similarity ≥ 60%.

3. **Diversity selection**  
   - Applying the MaxMin algorithm to select a diverse subset of compounds from the filtered set.

4. **Visualization**  
   - Displaying selected compounds in a **grid image** using RDKit's `MolsToGridImage`.

---

## **Installation**

```bash
# Create a virtual environment
python -m venv venv
source venv/bin/activate  # Linux/Mac
venv\Scripts\activate     # Windows

# Install required packages
pip install rdkit-pypi pandas
