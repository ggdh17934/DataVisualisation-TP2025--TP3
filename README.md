# DataVisualisation-TP2025 — TP3

Simple solution of the [teacher's TP3](https://github.com/ahmed3991/DataVisualisation-TP2025/blob/main/TP3/TP3.md), covering the required tasks only.

- **TP3.ipynb**: executed notebook, with real outputs and the written answers.
- **tp3.py**: equivalent Python entry point.
- **EXPLICATION_AR.md**: Arabic explanation of each step and the results.
- **data/**: the actual source data used.
- **results/**: generated results and **REPORT.md** with the required answers.

## Run

Download `TP3.ipynb` from this private repository, upload it to [Google Colab](https://colab.research.google.com/), and choose **Runtime → Run all**. The first cell installs missing libraries. Private GitHub links can require authentication; uploading the downloaded notebook avoids that issue.

Alternatively, from this repository folder:

```sh
python -m pip install -r requirements.txt
python tp3.py
```

Verified: all notebook cells executed successfully on 48,204 original UCI records. Required descriptive statistics, grouped tables, four plots and interpretation answers are included; the optional interactive bonus is omitted.
