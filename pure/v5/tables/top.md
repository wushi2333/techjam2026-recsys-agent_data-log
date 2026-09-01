# Highest valid primaries

| node | arm | primary | GAUC | nDCG@5 | Δ vs screen | patch |
|---|---|---|---|---|---|---|
| `071_ablate_c1_s0` | ablate | 0.60463 | 0.67099 | 0.53827 | 0.00077 | {"loss": "bpr_global", "seed": 0} |
| `160_finalize` | finalize | 0.60440 | 0.67105 | 0.53774 |  | finalize |
| `017_ensemble` | ensemble | 0.60440 | 0.67105 | 0.53774 | 0.00053 | ensemble:012_ablate_c1_s0,013_ablate_c1_s1,014_ablate_c1_s2 |
| `019_ensemble` | ensemble | 0.60438 | 0.67104 | 0.53773 | 0.00052 | ensemble:009_ablate_c0_s0,010_ablate_c0_s1,011_ablate_c0_s2,012_ablate_c1_s0,… |
| `095_ensemble` | ensemble | 0.60417 | 0.67041 | 0.53792 | 0.00031 | ensemble:088_ablate_c0_s0,089_ablate_c0_s1,090_ablate_c0_s2 |
| `016_ensemble` | ensemble | 0.60417 | 0.67062 | 0.53772 | 0.00031 | ensemble:009_ablate_c0_s0,010_ablate_c0_s1,011_ablate_c0_s2 |
| `018_ensemble` | ensemble | 0.60417 | 0.67062 | 0.53772 | 0.00031 | ensemble:009_ablate_c0_s0,010_ablate_c0_s1,011_ablate_c0_s2,012_ablate_c1_s0,… |
| `029_ensemble` | ensemble | 0.60417 | 0.67062 | 0.53772 | 0.00031 | ensemble:009_ablate_c0_s0,010_ablate_c0_s1,011_ablate_c0_s2,024_ablate_c1_s0,… |
| `042_ensemble` | ensemble | 0.60417 | 0.67062 | 0.53772 | 0.00031 | ensemble:009_ablate_c0_s0,010_ablate_c0_s1,011_ablate_c0_s2,024_ablate_c1_s0,… |
| `053_ensemble` | ensemble | 0.60417 | 0.67062 | 0.53772 | 0.00031 | ensemble:009_ablate_c0_s0,010_ablate_c0_s1,011_ablate_c0_s2,024_ablate_c1_s0,… |
| `065_ensemble` | ensemble | 0.60417 | 0.67062 | 0.53772 | 0.00031 | ensemble:009_ablate_c0_s0,010_ablate_c0_s1,011_ablate_c0_s2,024_ablate_c1_s0,… |
| `076_ensemble` | ensemble | 0.60417 | 0.67062 | 0.53772 | 0.00031 | ensemble:009_ablate_c0_s0,010_ablate_c0_s1,011_ablate_c0_s2,024_ablate_c1_s0,… |
| `086_ensemble` | ensemble | 0.60417 | 0.67062 | 0.53772 | 0.00031 | ensemble:009_ablate_c0_s0,010_ablate_c0_s1,011_ablate_c0_s2,024_ablate_c1_s0,… |
| `096_ensemble` | ensemble | 0.60417 | 0.67062 | 0.53772 | 0.00031 | ensemble:009_ablate_c0_s0,010_ablate_c0_s1,011_ablate_c0_s2,024_ablate_c1_s0,… |
| `031_capacity` | capacity | 0.60414 | 0.67084 | 0.53744 | 0.00028 | {"k": 8} |
| `105_ensemble` | ensemble | 0.60413 | 0.67035 | 0.53791 | 0.00018 | ensemble:098_ablate_c0_s0,099_ablate_c0_s1,100_ablate_c0_s2 |
| `106_ensemble` | ensemble | 0.60413 | 0.67035 | 0.53791 | 0.00018 | ensemble:009_ablate_c0_s0,010_ablate_c0_s1,011_ablate_c0_s2,024_ablate_c1_s0,… |
| `085_ensemble` | ensemble | 0.60410 | 0.67032 | 0.53787 | 0.00023 | ensemble:078_ablate_c0_s0,079_ablate_c0_s1,080_ablate_c0_s2 |
| `011_ablate_c0_s2` | ablate | 0.60407 | 0.67049 | 0.53765 | 0.00263 | {"arch": "deepfm", "seed": 2} |
| `026_ablate_c1_s2` | ablate | 0.60407 | 0.67049 | 0.53765 | 0.00021 | {"arch": "deepfm", "seed": 2} |
| `064_ensemble` | ensemble | 0.60403 | 0.67018 | 0.53787 | 0.00016 | ensemble:057_ablate_c0_s0,058_ablate_c0_s1,059_ablate_c0_s2 |
| `041_ensemble` | ensemble | 0.60402 | 0.67028 | 0.53777 | 0.00016 | ensemble:034_ablate_c0_s0,035_ablate_c0_s1,036_ablate_c0_s2 |
| `110_ablate_c0_s2` | ablate | 0.60402 | 0.67048 | 0.53756 | 0.00007 | {"seed": 2, "seq_len": 100, "seq_mode": "pool"} |
| `099_ablate_c0_s1` | ablate | 0.60399 | 0.67033 | 0.53764 | 0.00013 | {"seed": 1, "seq_len": 50, "seq_mode": "din"} |
| `102_ablate_c1_s1` | ablate | 0.60399 | 0.67033 | 0.53764 | 0.00013 | {"arch": "deepfm", "seed": 1} |
