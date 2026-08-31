# Highest valid primaries

| node | arm | primary | GAUC | nDCG@5 | Δ vs screen | patch |
|---|---|---|---|---|---|---|
| `159_finalize` | finalize | 0.63975 | 0.71748 | 0.56202 |  | finalize |
| `143_ensemble` | ensemble | 0.63931 | 0.71686 | 0.56177 | 0.00239 | ensemble:139_ablate_c0_s0,140_ablate_c0_s1,141_ablate_c0_s2 |
| `144_ensemble` | ensemble | 0.63931 | 0.71686 | 0.56177 | 0.00000 | ensemble:105_ablate_c0_s0,106_ablate_c0_s1,107_ablate_c0_s2,139_ablate_c0_s0,… |
| `112_ensemble` | ensemble | 0.63692 | 0.71361 | 0.56023 | 0.00307 | ensemble:105_ablate_c0_s0,106_ablate_c0_s1,107_ablate_c0_s2 |
| `113_ensemble` | ensemble | 0.63692 | 0.71361 | 0.56023 | 0.00000 | ensemble:025_ablate_c0_s0,026_ablate_c0_s1,027_ablate_c0_s2,032_ablate_c0_s0,… |
| `141_ablate_c0_s2` | ablate | 0.63635 | 0.71283 | 0.55987 | 0.00250 | {"aux_click": true, "seed": 2} |
| `138_multitask` | multitask | 0.63558 | 0.71275 | 0.55841 | 0.00173 | {"aux_click": true} |
| `139_ablate_c0_s0` | ablate | 0.63558 | 0.71275 | 0.55841 | 0.00173 | {"aux_click": true, "seed": 0} |
| `146_loss` | loss | 0.63558 | 0.71275 | 0.55841 | 0.00053 | {"bpr_pairs_cap": 64} |
| `150_loss` | loss | 0.63558 | 0.71275 | 0.55841 | 0.00053 | {"bpr_pairs_cap": 16} |
| `133_ablate_c0_s2` | ablate | 0.63557 | 0.71140 | 0.55974 | 0.00172 | {"seed": 2, "use_hour": true} |
| `136_ablate_c1_s2` | ablate | 0.63557 | 0.71140 | 0.55974 | 0.00172 | {"bpr_decay_sample": true, "seed": 2} |
| `130_time_shift` | time_shift | 0.63508 | 0.71085 | 0.55931 | 0.00123 | {"use_hour": true} |
| `131_ablate_c0_s0` | ablate | 0.63508 | 0.71085 | 0.55931 | 0.00123 | {"seed": 0, "use_hour": true} |
| `134_ablate_c1_s0` | ablate | 0.63508 | 0.71085 | 0.55931 | 0.00123 | {"bpr_decay_sample": true, "seed": 0} |
| `107_ablate_c0_s2` | ablate | 0.63495 | 0.71007 | 0.55984 | 0.00324 | {"arch": "dcnv2", "seed": 2} |
| `110_ablate_c1_s2` | ablate | 0.63495 | 0.71007 | 0.55984 | 0.00324 | {"bpr_pairs_cap": 64, "seed": 2} |
| `106_ablate_c0_s1` | ablate | 0.63356 | 0.70934 | 0.55779 | 0.00185 | {"arch": "dcnv2", "seed": 1} |
| `109_ablate_c1_s1` | ablate | 0.63356 | 0.70934 | 0.55779 | 0.00185 | {"bpr_pairs_cap": 64, "seed": 1} |
| `090_ablate_c0_s2` | ablate | 0.63337 | 0.71040 | 0.55633 | 0.00764 | {"k": 8, "seed": 2} |
| `092_ensemble` | ensemble | 0.63335 | 0.71030 | 0.55640 | 0.00163 | ensemble:088_ablate_c0_s0,089_ablate_c0_s1,090_ablate_c0_s2 |
| `093_ensemble` | ensemble | 0.63335 | 0.71030 | 0.55640 | 0.00000 | ensemble:025_ablate_c0_s0,026_ablate_c0_s1,027_ablate_c0_s2,032_ablate_c0_s0,… |
| `103_ensemble` | ensemble | 0.63335 | 0.71030 | 0.55640 | 0.00000 | ensemble:025_ablate_c0_s0,026_ablate_c0_s1,027_ablate_c0_s2,032_ablate_c0_s0,… |
| `140_ablate_c0_s1` | ablate | 0.63321 | 0.70872 | 0.55771 | -0.00063 | {"aux_click": true, "seed": 1} |
| `104_architecture` | architecture | 0.63303 | 0.70817 | 0.55788 | 0.00131 | {"arch": "dcnv2"} |
