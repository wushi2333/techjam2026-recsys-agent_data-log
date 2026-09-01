# Submitted Pure (`pure/v6`)

3-seed rank average of DeepFM + `seq_len=100` pool + `l2=1e-5` + logloss. Search used train + valid only. Finalize retrained members `059` / `060` / `061` on train.

| | GAUC | nDCG@5 | primary | vs FM |
|---|---|---|---|---|
| Official FM (valid) | 0.6674 | 0.5357 | 0.6016 | — |
| Submitted Pure (valid) | 0.67099 | 0.53816 | **0.60458** | **+0.00298** |
| Official FM (hidden test) | 0.6610 | 0.5282 | 0.5946 | — |
| Submitted Pure (hidden, once after search) | 0.66528 | 0.53137 | **0.59833** | **+0.00373** |

| | |
|---|---|
| Billed iterations | 50 / 50 |
| Wall-clock | **1.87 h** |
| Tokens in / out | **513,033 / 12,224** (525,257 total) |
| GPU-hours (harness field) | 0 |
| Runtime interventions | 0 |
| CSV rows | 170,588 |

Search incumbent at stop was `045` (DeepFM + seq-100 pool, confirmed mean 0.60396). Finalize’s bag rule preferred the l2 three-seed. Hidden test was scored once after search and was not used to pick the model.

A second freeze-eval search ([`../v5/`](../v5/)) independently shipped DeepFM + BPR and also beat the official FM.

## Files

| File | What it is |
|---|---|
| `submission.csv` | **Contest** scores, kit test order |
| `progress.log` | Readable trace |
| `journal.jsonl` | Hypothesis / patch / metrics |
| `changelog.jsonl` | Code/config diffs |
| `tables/trials.csv` | Flattened journal |
| `tables/top.md` | Highest valid primaries |
| `tables/confirmed.md` | Confirmed 3-seed identities |
| `tables/skips.md` | Duplicates and empty arms |
| `members/` | `trial_config.json` + `curves.csv` for FM, DeepFM+BPR, seq-100, contest bag |
| `dashboard.html` | Frozen status page from the run |
| `run_facts.md` | Harness-written facts (not a human agenda) |
| `results.json` | Valid table plus hidden diagnostic |

`log_random` in `results.json` is an off-policy check, not the kit random baseline, and was not used to pick the model. `summary.json` `integrity.src_hash` is `193172377e3a5ad4` at start and end (`unchanged=true`).
