# disease_trajectory_predictive_ML

Project notebook and cohort CSVs for event-sequence analysis and predictive modeling of gastric cancer.

Files in this folder:

- [Event_sequence_analysis_012826.ipynb](Event_sequence_analysis_012826.ipynb) — main analysis notebook (sequence building, stats, and models).
- [gastric_cancer_dcn_3l_v2.csv](gastric_cancer_dcn_3l_v2.csv) — gastric cancer cohort data used by the notebook.
- [non_gastric_cancer_dcn_3l_v2.csv](non_gastric_cancer_dcn_3l_v2.csv) — non-gastric cohort data used by the notebook.
- [requirements.txt](requirements.txt) — Python dependencies for running the notebook (includes `xgboost` and `lightgbm`).

Quick start

1. Create and activate a virtual environment:

```bash
python -m venv .venv
source .venv/bin/activate
```

2. Install dependencies:

```bash
pip install -r requirements.txt
```

3. Launch the notebook server and open the notebook:

```bash
jupyter notebook Event_sequence_analysis_012826.ipynb
```

Notes

- The notebook reads an Excel file named `gastric_sig_pairs_121525.xlsx` in one cell; that file is not included here. If you need to run the sequence-generation cells, provide that file or skip those cells.
- `openpyxl` is included to support reading Excel files via `pandas.read_excel()`.

If you want, I can also run the dependency installation now in this environment.