# Leaky Pure (`pure/v4`, not submitted)

The write-up calls this a useful failure. Recency features could read valid `long_view`, and missing test labels were stored as **0**. Valid primary went to **0.63975**. The same CSV, scored once afterwards, was **0.56790** on test — below the official FM 0.5946.

| | valid | after-the-fact test |
|---|---|---|
| primary | 0.63975 | 0.56790 |
| GAUC | 0.71748 | 0.62231 |
| nDCG@5 | 0.56202 | 0.51350 |

`submission.leaky.csv` is that test-score file (170,588 rows). **Do not submit it.** Hidden labels are not in this folder.

Members of the leaky blend: `139`–`141` and `088`–`090`. Configs and curves are under `members/`.

v5 rebuilt label handling (`-1` for missing, train-only decay) and is the contest CSV.
