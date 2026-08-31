# Pure v5 — contest run

3-seed rank average of `loss=bpr_global` on the numpy FM (DeepFM parent). Search used train + valid only. Finalize retrained members `012` / `013` / `014` on train.

| | GAUC | nDCG@5 | primary |
|---|---|---|---|
| Official FM (valid) | 0.6674 | 0.5357 | 0.6016 |
| This bag (valid) | 0.67105 | 0.53774 | **0.60440** |

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
| `submission.csv` | Contest scores, kit test order |
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
