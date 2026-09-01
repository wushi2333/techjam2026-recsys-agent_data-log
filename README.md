# KuaiRand run logs — TechJam 2026 Track 2

> **Contest file:** [`pure/v6/submission.csv`](pure/v6/submission.csv) (170,588 rows).  
> Code and write-up: [wushi2333/techjam2026-recsys-agent](https://github.com/wushi2333/techjam2026-recsys-agent).  
> Walkthrough (~3 min): [https://youtu.be/UvwHHWfqQhs](https://youtu.be/UvwHHWfqQhs).

This repo is the training record the code tree does not host: extra tables, full journals, the leaky v4 evidence, a second freeze-eval Pure search, and the 4.1M-row **KuaiRand-1K** CSV.

This is **not** the KuaiRand dataset. Raw logs stay on [Zenodo](https://zenodo.org/records/10439422). Hidden test labels are **not** here.

## Results

KuaiRand-Pure — label `long_view`, primary = mean(GAUC, nDCG@5). Kit `evaluate.py` unchanged.

| | GAUC | nDCG@5 | primary | vs FM |
|---|---|---|---|---|
| Official FM (valid) | 0.6674 | 0.5357 | 0.6016 | — |
| **Submitted Pure (valid)** DeepFM + seq-100 + l2 | 0.67099 | 0.53816 | **0.60458** | **+0.00298** |
| Official FM (hidden test) | 0.6610 | 0.5282 | 0.5946 | — |
| **Submitted Pure (hidden test)** | 0.66528 | 0.53137 | **0.59833** | **+0.00373** |
| Leaky Pure (valid) | 0.71748 | 0.56202 | 0.63975 | inflated |
| Leaky CSV (hidden test, once after search) | 0.62231 | 0.51350 | 0.56790 | worse than FM |

Hidden test on the contest CSV was scored **once after search** and was not used to pick the model.

A second freeze-eval Pure search independently shipped DeepFM + BPR and also beat the official FM (valid **0.60440** / hidden **0.59766**). Same parent scorer, same gates — not the contest CSV.

KuaiRand-1K is optional and uses a **different id space**. Do not compare it to Pure.

| | GAUC | nDCG@5 | primary | vs 1K FM |
|---|---|---|---|---|
| Official FM (1K valid) | 0.67461 | 0.60944 | 0.64203 | — |
| **Bonus 1K (valid)** train-only `use_time_decay` | 0.67654 | 0.62348 | **0.65001** | **+0.00798** |

| | Submitted Pure | Repeat Pure search | Leaky Pure (not submitted) | Bonus 1K |
|---|---|---|---|---|
| Folder | [`pure/v6/`](pure/v6/) | [`pure/v5/`](pure/v5/) | [`pure/v4/`](pure/v4/) | [`1k/`](1k/) |
| Recipe | DeepFM + seq-100 + l2 | DeepFM + BPR | leaky recency | FM + train-only decay |
| Billed iterations | 50 / 50 | 50 / 50 | 50 / 50 | 31 / 50 |
| Stop | cap | cap | cap | 6 h wall |
| Wall-clock | **1.87 h** | 2.91 h | 3.66 h | 6.50 h |
| Tokens in / out | **513,033 / 12,224** | 862,773 | 867,815 | 496,180 |
| Runtime interventions | **0** | **0** | 0 | **0** |
| Test rows in CSV | 170,588 | 170,588 | 170,588 | 4,132,081 |

Leaky Pure looked strong on valid because recency features could see valid labels, and missing test labels were stored as 0. Submitted Pure stores unseen labels as missing (`-1`) and updates decay / last-k from **train only**.

## Open first

| Path | What it is |
|---|---|
| [`pure/v6/submission.csv`](pure/v6/submission.csv) | **Contest** Pure scores (170,588 rows) |
| [`pure/v6/tables/top.md`](pure/v6/tables/top.md) | Highest submitted-Pure valid primaries |
| [`pure/v6/tables/trials.csv`](pure/v6/tables/trials.csv) | Every submitted-Pure journal node |
| [`pure/v6/progress.log`](pure/v6/progress.log) | Readable submitted-Pure trace |
| [`pure/v6/journal.jsonl`](pure/v6/journal.jsonl) | Hypothesis, patch, metrics per node |
| [`pure/v5/`](pure/v5/) | Repeat freeze-eval (DeepFM + BPR; not the contest CSV) |
| [`pure/v4/`](pure/v4/) | Leaky run evidence (not the contest CSV) |
| [`1k/submission.csv`](1k/submission.csv) | Bonus 1K scores (4.1M rows, Git LFS) |
| [`1k/submission.csv.gz`](1k/submission.csv.gz) | Same CSV, gzip (~40 MB, no LFS) |
| [`1k/tables/top.md`](1k/tables/top.md) | Highest 1K valid primaries |

## Layout

```
pure/v6/     Submitted Pure (run_pure_v6) — contest CSV
pure/v5/     Repeat freeze-eval (run_pure_v5) — DeepFM + BPR
pure/v4/     Leaky Pure (run_pure_v4) — evidence only
1k/          Bonus 1K (run_1k_aug31)
```

Each run folder has the journal, progress log, cost / status JSON, a `tables/` slice, and (where we had them) member `trial_config.json` + `curves.csv`. Member folders do **not** include `.npz` score dumps.

## What is not here

- KuaiRand raw `log_*.csv` / feature files — [Zenodo 10439422](https://zenodo.org/records/10439422)
- `hidden_test.json`, `infer_scores.npz`, `scores.npz`
- Trial source copies (`train.py`, …) — those live in the code repo `templates/`
- `.env` / API keys
- 27K (not attempted)

## Download the 1K CSV

GitHub rejects files over 100 MB in a normal blob, so the uncompressed 1K file is stored with **Git LFS**.

```bash
git lfs install
git clone https://github.com/wushi2333/techjam2026-recsys-agent_data-log.git
# or, without LFS:
curl -L -o submission.csv.gz https://github.com/wushi2333/techjam2026-recsys-agent_data-log/raw/main/1k/submission.csv.gz
gzip -d submission.csv.gz
```

SHA-256 checksums are in [`CHECKSUMS.md`](CHECKSUMS.md).

## Code and write-up

- Harness + Pure contest CSV: https://github.com/wushi2333/techjam2026-recsys-agent
- Longer notes: [`docs/report.md`](https://github.com/wushi2333/techjam2026-recsys-agent/blob/main/docs/report.md) in that repo

## License

Logs and tables in this repo: MIT, same as the code. KuaiRand itself stays under its own terms. Do not treat these CSVs as a redistribution of the dataset.
