# Bonus 1K

Optional scale. **Not** the contest primary. User and item ids are re-indexed, so these numbers are not comparable with Pure.

The loop is the same as submitted Pure. The **recipe is not**: contest Pure is 3-seed DeepFM + seq-100 + l2; this CSV is 3-seed train-only `use_time_decay` on FM. Search stopped on the 6 h wall at **31 / 50** billed iterations. Finalize retrained the confirmed bag (`039`, `040`, `041`) on train.

| | GAUC | nDCG@5 | primary | vs 1K FM |
|---|---|---|---|---|
| Official FM (1K) | 0.67461 | 0.60944 | 0.64203 | — |
| Finalize 3-seed rank average | 0.67654 | 0.62348 | **0.65001** | **+0.00798** |

Search bag valid was 0.65045; retrain drifted **−0.00044**. Alignment: **4,132,081** test rows.

| | |
|---|---|
| Billed iterations | 31 / 50 |
| Stop | `wall_clock` (6.50 h) |
| Tokens in + out | 496,180 |
| Runtime interventions | 0 |

`report.json` still prints `delta_vs_baseline` against Pure’s FM (0.6016). Use **+0.00798** vs the 1K FM above.

A later 1-seed DCNv2 (0.65280) never got a 3-seed because the clock ran out; it is not in the CSV.

Contest Pure: [`../pure/v6/`](../pure/v6/).

## Files

| File | What it is |
|---|---|
| `submission.csv` | 4.1M-row scores (Git LFS, ~117 MB) |
| `submission.csv.gz` | Same file, gzip (~40 MB) |
| `progress.log` | Readable trace |
| `journal.jsonl` | Hypothesis / patch / metrics |
| `tables/trials.csv` | Flattened journal |
| `tables/top.md` | Highest valid primaries |
| `report.json` | Finalize summary |
| `metrics.json` | Valid GAUC / nDCG / primary |

Trial folders from AutoDL were not copied (too large, include `.npz`). The journal is the complete search record.
