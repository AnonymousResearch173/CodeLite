# CodeLite

This repository contains the implementation and experimental artifacts for **CodeLite**, a lightweight hybrid framework for source code classification tasks based on enhanced code representations and lexical fusion techniques.

The repository is provided to support the reproducibility of the experiments reported in the associated manuscript.

---

# Repository Structure

```text
CodeLite/
│
├── PLI/
├── PLAG/
├── Authorship/
├── Ablations_and_Additional_Tests/
└── README.md
```

## PLI

Contains notebooks related to **Programming Language Identification (PLI)** experiments.

Files included:

* `codelite.ipynb`
* `Mistral_PLI.ipynb`
* `codellama_PLI.ipynb`
* `codet5_PLI.ipynb`

---

## PLAG

Contains notebooks related to **source code plagiarism detection** experiments.

Files included:

* `CodeLite_Plag.ipynb`
* `codellama_plag.ipynb`
* `codet5+_plag.ipynb`
* `deepseekcoder_plag.ipynb`

---

## Authorship

Contains notebooks related to **source code authorship attribution** experiments.

Files included:

* `CodeLite_Authorship.ipynb`
* `Authorship_codellamma.ipynb`
* `Authorship_deepseekcoder.ipynb`
* `codet5+_authorship.ipynb`

---

## Ablations_and_Additional_Tests

Contains notebooks for:

* ablation studies,
* representation layer information (RI) analysis,
* lightweight PTM analysis,
* baseline comparisons,
* additional experimental evaluations.

Files included:

* `BERT_RI_Approach.ipynb`
* `codet5_RI_Approach.ipynb`
* `graphcodebert_RI_Approach.ipynb`
* `unixcoder_RI_Approach.ipynb`
* `TF_IDF_Regex_Ablation.ipynb`
* `Stage_1_vs_Stage_2.ipynb`
* `Traditional_Models.ipynb`
* `Code_2_Vec.ipynb`
* `ast_gnn.ipynb`
* `lightweight_ptms.ipynb`

---

# Dataset Access

The datasets used in this work are publicly available through Zenodo:

https://zenodo.org/records/20429617

The dataset package includes:

## Programming Language Identification (PLI)

* `train.csv`
* `test.csv`
* `unique_tags.csv`

## Source Code Plagiarism Detection

* `train.csv`
* `test_0.csv` to `test_9.csv`

## Source Code Authorship Attribution

* `Authorship.csv`

---

# Environment Setup

We recommend Python 3.10 or later.

## Clone the Repository

```bash
git clone <repository_link>
cd CodeLite
```

## Create a Virtual Environment

```bash
python -m venv codelite_env
```

### Linux/macOS

```bash
source codelite_env/bin/activate
```

### Windows

```bash
codelite_env\Scripts\activate
```

## Install Dependencies

```bash
pip install torch transformers scikit-learn pandas numpy matplotlib jupyter
```

---

# Reproducing the Experiments

All experiments are provided as Jupyter notebooks.

After downloading the datasets from Zenodo, place the dataset files in the appropriate paths expected by the notebooks and execute the notebook cells sequentially.

Each notebook contains the complete implementation pipeline corresponding to its respective experiment.

---

# Citation

If you use this repository or dataset in your research, please cite the associated paper.
