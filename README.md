# Experimental data

Each CSV represents one experiment group and contains all 20 archived runs. The file names identify the group. Columns give the original recorded time and signal value. The `sample_index` restarts at 1 for each run. Separate time columns preserve each signal's recorded timestamps. Units are in the column names.

| File-name pattern | Experiment | Controller |
| --- | --- | --- |
| `startup_prop_etaXX.csv` | Loaded startup | Proposed, smoothing factor `XX/10` |
| `startup_basic_etaXX.csv` | Loaded startup | Basic seven-vector method, smoothing factor `XX/10` |
| `step_prop_etaXX.csv` | 0-to-1-N·m load step | Proposed, smoothing factor `XX/10` |
| `step_basic_etaXX.csv` | 0-to-1-N·m load step | Basic seven-vector method, smoothing factor `XX/10` |
| `step_kawai.csv` | 0-to-1-N·m load step | VS-MPDSC, `K_a=0.85` |
| `step_zerdali.csv` | 0-to-1-N·m load step | WFF-PDSC |
| `large_prop_etaXX.csv` | Large-smoothing startup and load step | Proposed, smoothing factor `XX/10` |
| `robust_R_*.csv` | Stator-resistance mismatch | Controller indicated by suffix |
| `robust_L_*.csv` | Stator-inductance mismatch | Controller indicated by suffix |
| `robust_psi_*.csv` | Flux-linkage mismatch | Controller indicated by suffix |

`prop`, `kawai`, and `zerdali` in robustness file names denote Proposed, VS-MPDSC (`K_a=0.85`), and WFF-PDSC. The suffix `XX` uses `00`, `03`, `04`, `06`, `07`, `08`, or `09` as applicable.