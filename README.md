# PROTEIN-STRUCTURE-MODELLING-SWISS-MODELLING--2DN1-Human-Hemoglobin.
PROTEIN-STRUCTURE-MODELLING [SWISS MODELLING]-2DN1 = 1.25A resolution crystal structure of human hemoglobin in the oxy form
# Homology Modeling: Human Hemoglobin Alpha Subunit (HBA) Structure Prediction 🧬🔬

## Overview

This repository contains the complete results of a **Homology Modeling** project performed using the **SWISS-MODEL Server**. The goal was to generate a highly accurate 3D structural model of the **Human Hemoglobin Alpha Subunit (HBA)**, based on a sequence labeled `2DN1 mutated,fasta`.

The prediction successfully generated a model, utilizing the high similarity to the experimentally solved Hemoglobin structure (PDB ID: **2DN2**) to ensure high confidence in the predicted structure.

---

## Target System and Methodology

* **Target Protein:** Hemoglobin alpha subunit (HBA), *Homo sapiens*.
* **Target Sequence ID:** `2DN1 mutated,fasta` (Hemoglobin alpha subunit).
* **Modeling Tool:** SWISS-MODEL Server.
* **Key Template Used:** PDB ID **2dn2.1.C** (Hemoglobin alpha subunit), showing a very high sequence identity of **99.29%**.
* **Predicted Oligo-State:** **Monomer** (model of a single subunit).
* **Key Ligand:** The model includes the Heme group (**HEM**), which is essential for oxygen binding.

### Key Model Quality Metrics

The high quality of the prediction is confirmed by the following metrics (derived from `model_01.json` and reports):

| Metric | Value | Interpretation |
| :--- | :--- | :--- |
| **Global Model Quality Estimate (GMQE)** | **0.91** | Excellent score (closer to 1.0 is better), suggesting high reliability of the overall fold. |
| **QMEANDisCo Global** | $\mathbf{0.84 \pm 0.07}$ | High score, confirming the global model quality is comparable to high-resolution experimental structures. |
| **Template Identity** | **99.29%** | Near-perfect sequence match to the top template, guaranteeing high structural accuracy. |

---

## Repository Files

The files are categorized into the final structural output, raw inputs, and detailed quality reports:

| File Name | Description | Category |
| :--- | :--- | :--- |
| **model\_01.pdb** | **The final predicted 3D structure** of the Hemoglobin Alpha Subunit, including the Heme group. | Output |
| `model_01.json` | Detailed JSON file containing all structural and quality assessment data (QMEAN, Z-scores). | Output/Metrics |
| `report.html` | The full, interactive **SWISS-MODEL report**, containing all visualization charts, sequence alignment, and detailed metrics. | Report |
| `2DN1 mutated,fasta _ Summary.pdf` | Summary report including target sequence, template filtering results, and global quality metrics. | Report |
| `2DN1 mutated,fasta _ Models.pdf` | Report containing residue-by-residue local quality estimates and alignment details. | Report |
| `rcsb_pdb_2DN1.fasta` | Fasta file of the original 2DN1 protein, used as input sequence source. | Input |
| `Local_quality_estimate.png` | Graphical representation of the residue-by-residue local quality score (QMEANDisCo). | Visualization |
| `Quality_comparison.png` | Graph comparing the model's overall quality against experimental structures. | Visualization |
| `2dn2.1.pdb` | The PDB file for the top template used (2DN2). | Context |

---

## Setup and Usage

1.  **Clone the repository:**
    ```bash
    git clone [Your Repository URL]
    cd [Your Repository Name]
    ```

2.  **View the 3D Model:**
    Load the **`model_01.pdb`** file into any molecular visualization software (e.g., **PyMOL**, **ChimeraX**, or **VMD**) to inspect the predicted HBA subunit structure and the bound Heme molecule.

3.  **Review the Full Report:**
    Open the **`report.html`** file in a web browser to view the interactive quality assessment, detailed template alignments, and residue-specific confidence scores.
