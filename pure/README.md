# Pure

Contest primary is **KuaiRand-Pure**. Folder split:

| Folder | Name | Role |
|---|---|---|
| [`v6/`](v6/) | **Submitted Pure** (`run_pure_v6`) | Contest CSV. 3-seed DeepFM + seq-100 + l2, valid **0.60458** / hidden **0.59833**. |
| [`v5/`](v5/) | Repeat freeze-eval (`run_pure_v5`) | DeepFM + BPR, also above the official FM. **Not** the contest CSV. |
| [`v4/`](v4/) | **Leaky Pure** (`run_pure_v4`) | Valid 0.63975, after-the-fact test 0.56790. **Not submitted.** |

Do not mix the CSVs. Judges scoring a file should use [`v6/submission.csv`](v6/submission.csv).
