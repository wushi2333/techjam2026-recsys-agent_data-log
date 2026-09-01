# Repeat freeze-eval Pure (`pure/v5`)

**Not** the contest CSV. A second freeze-eval search that independently shipped 3-seed DeepFM + `loss=bpr_global` and also beat the official FM. Search used train + valid only. Finalize retrained members `012` / `013` / `014` on train.

Contest file: [`../v6/submission.csv`](../v6/submission.csv).

| | GAUC | nDCG@5 | primary | vs FM |
|---|---|---|---|---|
| Official FM (valid) | 0.6674 | 0.5357 | 0.6016 | — |
| Repeat bag (valid) | 0.67105 | 0.53774 | **0.60440** | **+0.00280** |
| Official FM (hidden test) | 0.6610 | 0.5282 | 0.5946 | — |
| Repeat CSV (hidden, once after search) | 0.66486 | 0.53046 | **0.59766** | **+0.00306** |

| | |
|---|---|
| Billed iterations | 50 / 50 |
| Wall-clock | 2.91 h |
| Tokens in + out | 862,773 |
| GPU-hours (harness field) | 0 |
| Runtime interventions | 0 |
| CSV rows | 170,588 |

Search incumbent at stop was `098` (DeepFM + DIN-50, mean 0.60395). Finalize’s bag rule preferred the BPR three-seed.

## Files

| File | What it is |
|---|---|
| `submission.csv` | Repeat-search scores (not the contest file) |
| `progress.log` | Readable trace |
| `journal.jsonl` | Hypothesis / patch / metrics |
| `changelog.jsonl` | Code/config diffs |
| `tables/trials.csv` | Flattened journal |
| `tables/top.md` | Highest valid primaries |
| `tables/confirmed.md` | Confirmed 3-seed identities |
| `tables/skips.md` | Duplicates and empty arms |
| `members/` | `trial_config.json` + `curves.csv` for FM, DeepFM, BPR, DIN-50 |
| `dashboard.html` | Frozen status page from the run |
| `run_facts.md` | Harness-written facts (not a human agenda) |

`log_random` in `results.json` is an off-policy check, not the kit random baseline, and was not used to pick the model.
