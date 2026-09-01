# Highest valid primaries

| node | arm | primary | GAUC | nDCG@5 | Δ vs screen | patch |
|---|---|---|---|---|---|---|
| `049_architecture` | architecture | 0.65280 | 0.67630 | 0.62940 | 0.00638 | {"arch": "dcnv2", "data_scale": "1k"} |
| `032_debug` | regularization | 0.65061 | 0.67918 | 0.62204 |  | config:l2 |
| `046_ensemble` | ensemble | 0.65045 | 0.67660 | 0.62429 | 0.00403 | ensemble:039_ablate_c0_s0,040_ablate_c0_s1,041_ablate_c0_s2 |
| `047_ensemble` | ensemble | 0.65045 | 0.67660 | 0.62429 | 0.00403 | ensemble:000_fm_baseline,000_fm_s1,001_fm_s2,015_ablate_c0_s0,016_ablate_c0_s… |
| `054_finalize` | finalize | 0.65001 | 0.67654 | 0.62348 |  | finalize |
| `038_features` | features | 0.64835 | 0.67567 | 0.62103 | 0.00497 | {"use_time_decay": true} |
| `039_ablate_c0_s0` | ablate | 0.64835 | 0.67567 | 0.62103 | 0.00497 | {"seed": 0, "use_time_decay": true} |
| `053_architecture` | architecture | 0.64580 | 0.67160 | 0.62000 | -0.00062 | {"arch": "deepfm", "data_scale": "1k"} |
| `040_ablate_c0_s1` | ablate | 0.64569 | 0.67507 | 0.61632 | 0.00231 | {"seed": 1, "use_time_decay": true} |
| `041_ablate_c0_s2` | ablate | 0.64522 | 0.67300 | 0.61744 | 0.00184 | {"seed": 2, "use_time_decay": true} |
| `016_ablate_c0_s1` | ablate | 0.64423 | 0.67461 | 0.61385 | 0.00248 | {"seed": 1, "seq_len": 100, "seq_mode": "din"} |
| `022_ensemble` | ensemble | 0.64401 | 0.67532 | 0.61269 | 0.00063 | ensemble:015_ablate_c0_s0,016_ablate_c0_s1,017_ablate_c0_s2 |
| `023_ensemble` | ensemble | 0.64401 | 0.67532 | 0.61269 | 0.00063 | ensemble:000_fm_baseline,000_fm_s1,001_fm_s2,015_ablate_c0_s0,016_ablate_c0_s… |
| `017_ablate_c0_s2` | ablate | 0.64356 | 0.67435 | 0.61277 | 0.00181 | {"seed": 2, "seq_len": 100, "seq_mode": "din"} |
| `024_ensemble` | ensemble | 0.64280 | 0.67535 | 0.61026 | -0.00058 | ensemble:000_fm_baseline,000_fm_s1,001_fm_s2,015_ablate_c0_s0,016_ablate_c0_s… |
| `000_fm_s1` | ablate | 0.64263 | 0.67458 | 0.61067 |  | {"aux_click_weight": 0.3, "cwm_weight": 0.2, "data_scale": "1k", "model_famil… |
| `014_sequence` | sequence | 0.64236 | 0.67515 | 0.60956 | 0.00061 | {"seq_len": 100, "seq_mode": "din"} |
| `015_ablate_c0_s0` | ablate | 0.64236 | 0.67515 | 0.60956 | 0.00061 | {"seed": 0, "seq_len": 100, "seq_mode": "din"} |
| `000_fm_baseline` | draft | 0.64203 | 0.67461 | 0.60944 |  | {"aux_click_weight": 0.3, "cwm_weight": 0.2, "data_scale": "1k", "model_famil… |
| `011_multitask` | multitask | 0.64203 | 0.67461 | 0.60944 | 0.00028 | {"aux_click": true} |
| `010_ensemble` | ensemble | 0.64181 | 0.67519 | 0.60843 | 0.00006 | ensemble:000_fm_baseline,000_fm_s1,001_fm_s2 |
| `001_fm_s2` | ablate | 0.64060 | 0.67439 | 0.60680 |  | {"aux_click_weight": 0.3, "cwm_weight": 0.2, "data_scale": "1k", "model_famil… |
| `012_capacity` | capacity | 0.64053 | 0.67569 | 0.60538 | -0.00122 | {"k": 32} |
| `036_architecture` | architecture | 0.63800 | 0.67280 | 0.60320 | -0.00538 | {"arch": "dcnv2", "data_scale": "1k"} |
| `013_watch_time` | watch_time | 0.63567 | 0.67196 | 0.59938 | -0.00608 | {"wlr_play": true} |
