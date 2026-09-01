# Highest valid primaries

| node | arm | primary | GAUC | nDCG@5 | Δ vs screen | patch |
|---|---|---|---|---|---|---|
| `061_ablate_c1_s2` | ablate | 0.60464 | 0.67132 | 0.53796 | 0.00068 | {"l2": 1e-05, "seed": 2} |
| `142_finalize` | finalize | 0.60458 | 0.67099 | 0.53816 |  | finalize |
| `063_ensemble` | ensemble | 0.60457 | 0.67099 | 0.53816 | 0.00062 | ensemble:059_ablate_c1_s0,060_ablate_c1_s1,061_ablate_c1_s2 |
| `064_ensemble` | ensemble | 0.60457 | 0.67099 | 0.53816 | 0.00062 | ensemble:009_ablate_c0_s0,010_ablate_c0_s1,011_ablate_c0_s2,022_ablate_c1_s0,… |
| `093_ensemble` | ensemble | 0.60457 | 0.67099 | 0.53816 | 0.00062 | ensemble:009_ablate_c0_s0,010_ablate_c0_s1,011_ablate_c0_s2,022_ablate_c1_s0,… |
| `114_ensemble` | ensemble | 0.60457 | 0.67099 | 0.53816 | 0.00062 | ensemble:009_ablate_c0_s0,010_ablate_c0_s1,011_ablate_c0_s2,022_ablate_c1_s0,… |
| `013_ensemble` | ensemble | 0.60441 | 0.67100 | 0.53782 | 0.00159 | ensemble:009_ablate_c0_s0,010_ablate_c0_s1,011_ablate_c0_s2 |
| `015_ensemble` | ensemble | 0.60441 | 0.67100 | 0.53782 | 0.00159 | ensemble:000_fm_baseline,000_fm_s1,001_fm_s2,009_ablate_c0_s0,010_ablate_c0_s… |
| `026_ensemble` | ensemble | 0.60440 | 0.67105 | 0.53774 | 0.00100 | ensemble:019_ablate_c0_s0,020_ablate_c0_s1,021_ablate_c0_s2 |
| `027_ensemble` | ensemble | 0.60440 | 0.67105 | 0.53774 | 0.00100 | ensemble:000_fm_baseline,000_fm_s1,001_fm_s2,009_ablate_c0_s0,010_ablate_c0_s… |
| `052_ensemble` | ensemble | 0.60438 | 0.67079 | 0.53797 | 0.00043 | ensemble:045_ablate_c0_s0,046_ablate_c0_s1,047_ablate_c0_s2 |
| `053_ensemble` | ensemble | 0.60438 | 0.67079 | 0.53797 | 0.00043 | ensemble:009_ablate_c0_s0,010_ablate_c0_s1,011_ablate_c0_s2,022_ablate_c1_s0,… |
| `088_ablate_c1_s0` | ablate | 0.60436 | 0.67080 | 0.53792 | 0.00041 | {"loss": "bpr_global", "seed": 0} |
| `059_ablate_c1_s0` | ablate | 0.60433 | 0.67074 | 0.53791 | 0.00037 | {"l2": 1e-05, "seed": 0} |
| `047_ablate_c0_s2` | ablate | 0.60402 | 0.67048 | 0.53756 | 0.00062 | {"seed": 2, "seq_len": 100, "seq_mode": "pool"} |
| `058_ablate_c0_s2` | ablate | 0.60402 | 0.67048 | 0.53756 | 0.00006 | {"seed": 2, "seq_len": 100, "seq_mode": "pool"} |
| `070_ablate_c0_s2` | ablate | 0.60402 | 0.67048 | 0.53756 | 0.00006 | {"seed": 2, "seq_len": 100, "seq_mode": "pool"} |
| `081_ablate_c0_s2` | ablate | 0.60402 | 0.67048 | 0.53756 | 0.00006 | {"seed": 2, "seq_len": 100, "seq_mode": "pool"} |
| `098_ablate_c0_s2` | ablate | 0.60402 | 0.67048 | 0.53756 | 0.00006 | {"seed": 2, "seq_len": 100, "seq_mode": "pool"} |
| `128_ablate_c0_s2` | ablate | 0.60402 | 0.67048 | 0.53756 | 0.00006 | {"seed": 2, "seq_len": 100, "seq_mode": "pool"} |
| `044_sequence` | sequence | 0.60396 | 0.67006 | 0.53786 | 0.00057 | {"seq_len": 100, "seq_mode": "pool"} |
| `045_ablate_c0_s0` | ablate | 0.60396 | 0.67006 | 0.53786 | 0.00057 | {"seed": 0, "seq_len": 100, "seq_mode": "pool"} |
| `056_ablate_c0_s0` | ablate | 0.60396 | 0.67006 | 0.53786 | 0.00000 | {"seed": 0, "seq_len": 100, "seq_mode": "pool"} |
| `068_ablate_c0_s0` | ablate | 0.60396 | 0.67006 | 0.53786 | 0.00000 | {"seed": 0, "seq_len": 100, "seq_mode": "pool"} |
| `079_ablate_c0_s0` | ablate | 0.60396 | 0.67006 | 0.53786 | 0.00000 | {"seed": 0, "seq_len": 100, "seq_mode": "pool"} |
