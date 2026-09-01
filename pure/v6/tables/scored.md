# Scored trials (valid primary, high → low)

Official FM on this scale is **0.60160**. Kit `evaluate.py` only.

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
| `096_ablate_c0_s0` | ablate | 0.60396 | 0.67006 | 0.53786 | 0.00000 | {"seed": 0, "seq_len": 100, "seq_mode": "pool"} |
| `126_ablate_c0_s0` | ablate | 0.60396 | 0.67006 | 0.53786 | 0.00000 | {"seed": 0, "seq_len": 100, "seq_mode": "pool"} |
| `007_draft` | draft | 0.60392 | 0.67040 | 0.53743 | 0.00248 | {"loss": "bpr_global"} |
| `009_ablate_c0_s0` | ablate | 0.60392 | 0.67040 | 0.53743 | 0.00248 | {"loss": "bpr_global", "seed": 0} |
| `022_ablate_c1_s0` | ablate | 0.60392 | 0.67040 | 0.53743 | 0.00110 | {"arch": "fm", "loss": "bpr_global", "seed": 0} |
| `046_ablate_c0_s1` | ablate | 0.60389 | 0.67008 | 0.53770 | 0.00049 | {"seed": 1, "seq_len": 100, "seq_mode": "pool"} |
| `057_ablate_c0_s1` | ablate | 0.60389 | 0.67008 | 0.53770 | -0.00007 | {"seed": 1, "seq_len": 100, "seq_mode": "pool"} |
| `069_ablate_c0_s1` | ablate | 0.60389 | 0.67008 | 0.53770 | -0.00007 | {"seed": 1, "seq_len": 100, "seq_mode": "pool"} |
| `080_ablate_c0_s1` | ablate | 0.60389 | 0.67008 | 0.53770 | -0.00007 | {"seed": 1, "seq_len": 100, "seq_mode": "pool"} |
| `097_ablate_c0_s1` | ablate | 0.60389 | 0.67008 | 0.53770 | -0.00007 | {"seed": 1, "seq_len": 100, "seq_mode": "pool"} |
| `127_ablate_c0_s1` | ablate | 0.60389 | 0.67008 | 0.53770 | -0.00007 | {"seed": 1, "seq_len": 100, "seq_mode": "pool"} |
| `016_ensemble` | ensemble | 0.60382 | 0.67039 | 0.53726 | 0.00100 | ensemble:000_fm_baseline,000_fm_s1,001_fm_s2,009_ablate_c0_s0,010_ablate_c0_s… |
| `060_ablate_c1_s1` | ablate | 0.60380 | 0.66998 | 0.53762 | -0.00016 | {"l2": 1e-05, "seed": 1} |
| `030_ablate_c0_s1` | ablate | 0.60374 | 0.67032 | 0.53715 | 0.00034 | {"arch": "dcnv2", "seed": 1} |
| `031_ablate_c0_s2` | ablate | 0.60369 | 0.67002 | 0.53736 | 0.00030 | {"arch": "dcnv2", "seed": 2} |
| `018_architecture` | architecture | 0.60362 | 0.66992 | 0.53733 | 0.00080 | {"arch": "deepfm"} |
| `019_ablate_c0_s0` | ablate | 0.60362 | 0.66992 | 0.53733 | 0.00080 | {"arch": "deepfm", "seed": 0} |
| `040_ablate_c0_s0` | ablate | 0.60362 | 0.66992 | 0.53733 | 0.00023 | {"arch": "deepfm", "seed": 0} |
| `036_ensemble` | ensemble | 0.60361 | 0.67007 | 0.53715 | 0.00021 | ensemble:029_ablate_c0_s0,030_ablate_c0_s1,031_ablate_c0_s2 |
| `037_ensemble` | ensemble | 0.60361 | 0.67007 | 0.53715 | 0.00021 | ensemble:009_ablate_c0_s0,010_ablate_c0_s1,011_ablate_c0_s2,022_ablate_c1_s0,… |
| `049_ablate_c1_s1` | ablate | 0.60360 | 0.67022 | 0.53697 | 0.00020 | {"loss": "bpr_global", "seed": 1} |
| `072_ablate_c1_s1` | ablate | 0.60360 | 0.67022 | 0.53697 | -0.00036 | {"loss": "bpr_global", "seed": 1} |
| `100_ablate_c1_s1` | ablate | 0.60360 | 0.67022 | 0.53697 | -0.00036 | {"loss": "bpr_global", "seed": 1} |
| `130_ablate_c1_s1` | ablate | 0.60360 | 0.67022 | 0.53697 | -0.00036 | {"loss": "bpr_global", "seed": 1} |
| `020_ablate_c0_s1` | ablate | 0.60356 | 0.67050 | 0.53663 | 0.00074 | {"arch": "deepfm", "seed": 1} |
| `041_ablate_c0_s1` | ablate | 0.60356 | 0.67050 | 0.53663 | 0.00017 | {"arch": "deepfm", "seed": 1} |
| `048_ablate_c1_s0` | ablate | 0.60352 | 0.66969 | 0.53734 | 0.00012 | {"loss": "bpr_global", "seed": 0} |
| `071_ablate_c1_s0` | ablate | 0.60352 | 0.66969 | 0.53734 | -0.00044 | {"loss": "bpr_global", "seed": 0} |
| `099_ablate_c1_s0` | ablate | 0.60352 | 0.66969 | 0.53734 | -0.00044 | {"loss": "bpr_global", "seed": 0} |
| `129_ablate_c1_s0` | ablate | 0.60352 | 0.66969 | 0.53734 | -0.00044 | {"loss": "bpr_global", "seed": 0} |
| `076_regularization` | regularization | 0.60327 | 0.66960 | 0.53694 | -0.00069 | {"l2": 5e-06} |
| `050_ablate_c1_s2` | ablate | 0.60321 | 0.67004 | 0.53639 | -0.00018 | {"loss": "bpr_global", "seed": 2} |
| `073_ablate_c1_s2` | ablate | 0.60321 | 0.67004 | 0.53639 | -0.00074 | {"loss": "bpr_global", "seed": 2} |
| `101_ablate_c1_s2` | ablate | 0.60321 | 0.67004 | 0.53639 | -0.00074 | {"loss": "bpr_global", "seed": 2} |
| `131_ablate_c1_s2` | ablate | 0.60321 | 0.67004 | 0.53639 | -0.00074 | {"loss": "bpr_global", "seed": 2} |
| `092_ensemble` | ensemble | 0.60317 | 0.66964 | 0.53671 | -0.00078 | ensemble:085_ablate_c0_s0,086_ablate_c0_s1,087_ablate_c0_s2 |
| `112_ensemble` | ensemble | 0.60308 | 0.66942 | 0.53674 | -0.00088 | ensemble:105_ablate_c0_s0,106_ablate_c0_s1,107_ablate_c0_s2 |
| `113_ensemble` | ensemble | 0.60308 | 0.66942 | 0.53674 | -0.00088 | ensemble:108_ablate_c1_s0,109_ablate_c1_s1,110_ablate_c1_s2 |
| `065_regularization` | regularization | 0.60306 | 0.66891 | 0.53721 | -0.00090 | {"l2": 1e-05} |
| `033_ablate_c1_s1` | ablate | 0.60305 | 0.66926 | 0.53684 | -0.00034 | {"loss": "bpr_global", "seed": 1} |
| `032_ablate_c1_s0` | ablate | 0.60301 | 0.66887 | 0.53714 | -0.00039 | {"loss": "bpr_global", "seed": 0} |
| `021_ablate_c0_s2` | ablate | 0.60300 | 0.66959 | 0.53640 | 0.00018 | {"arch": "deepfm", "seed": 2} |
| `042_ablate_c0_s2` | ablate | 0.60300 | 0.66959 | 0.53640 | -0.00040 | {"arch": "deepfm", "seed": 2} |
| `084_sequence` | sequence | 0.60295 | 0.66916 | 0.53674 | -0.00101 | {"seq_len": 50, "seq_mode": "pool"} |
| `085_ablate_c0_s0` | ablate | 0.60295 | 0.66916 | 0.53674 | -0.00101 | {"seed": 0, "seq_len": 50, "seq_mode": "pool"} |
| `104_sequence` | sequence | 0.60290 | 0.66906 | 0.53675 | -0.00105 | {"seq_len": 50, "seq_mode": "din"} |
| `105_ablate_c0_s0` | ablate | 0.60290 | 0.66906 | 0.53675 | -0.00105 | {"seed": 0, "seq_len": 50, "seq_mode": "din"} |
| `108_ablate_c1_s0` | ablate | 0.60290 | 0.66906 | 0.53675 | -0.00105 | {"loss": "logloss", "seed": 0} |
| `028_architecture` | architecture | 0.60289 | 0.66910 | 0.53669 | -0.00050 | {"arch": "dcnv2"} |
| `029_ablate_c0_s0` | ablate | 0.60289 | 0.66910 | 0.53669 | -0.00050 | {"arch": "dcnv2", "seed": 0} |
| `116_sequence` | sequence | 0.60280 | 0.66864 | 0.53695 | -0.00116 | {"seq_len": 20, "seq_mode": "pool"} |
| `117_ablate_c0_s0` | ablate | 0.60280 | 0.66864 | 0.53695 | -0.00116 | {"seed": 0, "seq_len": 20, "seq_mode": "pool"} |
| `120_ablate_c1_s0` | ablate | 0.60280 | 0.66864 | 0.53695 | -0.00116 | {"loss": "logloss", "seed": 0} |
| `086_ablate_c0_s1` | ablate | 0.60261 | 0.66888 | 0.53635 | -0.00134 | {"seed": 1, "seq_len": 50, "seq_mode": "pool"} |
| `103_sequence` | sequence | 0.60257 | 0.66874 | 0.53641 | -0.00138 | {"seq_len": 20, "seq_mode": "din"} |
| `010_ablate_c0_s1` | ablate | 0.60249 | 0.66865 | 0.53634 | 0.00105 | {"loss": "bpr_global", "seed": 1} |
| `023_ablate_c1_s1` | ablate | 0.60249 | 0.66865 | 0.53634 | -0.00033 | {"arch": "fm", "loss": "bpr_global", "seed": 1} |
| `106_ablate_c0_s1` | ablate | 0.60245 | 0.66868 | 0.53622 | -0.00151 | {"seed": 1, "seq_len": 50, "seq_mode": "din"} |
| `109_ablate_c1_s1` | ablate | 0.60245 | 0.66868 | 0.53622 | -0.00151 | {"loss": "logloss", "seed": 1} |
| `118_ablate_c0_s1` | ablate | 0.60229 | 0.66834 | 0.53624 | -0.00167 | {"seed": 1, "seq_len": 20, "seq_mode": "pool"} |
| `121_ablate_c1_s1` | ablate | 0.60229 | 0.66834 | 0.53624 | -0.00167 | {"loss": "logloss", "seed": 1} |
| `011_ablate_c0_s2` | ablate | 0.60205 | 0.66797 | 0.53612 | 0.00061 | {"loss": "bpr_global", "seed": 2} |
| `024_ablate_c1_s2` | ablate | 0.60205 | 0.66797 | 0.53612 | -0.00077 | {"arch": "fm", "loss": "bpr_global", "seed": 2} |
| `089_ablate_c1_s1` | ablate | 0.60200 | 0.66789 | 0.53611 | -0.00196 | {"loss": "bpr_global", "seed": 1} |
| `087_ablate_c0_s2` | ablate | 0.60197 | 0.66765 | 0.53628 | -0.00199 | {"seed": 2, "seq_len": 50, "seq_mode": "pool"} |
| `133_sequence` | sequence | 0.60191 | 0.66758 | 0.53624 | -0.00204 | {"seq_len": 10, "seq_mode": "pool"} |
| `014_ensemble` | ensemble | 0.60189 | 0.66766 | 0.53612 | -0.00093 | ensemble:000_fm_baseline,000_fm_s1,001_fm_s2 |
| `107_ablate_c0_s2` | ablate | 0.60185 | 0.66797 | 0.53573 | -0.00211 | {"seed": 2, "seq_len": 50, "seq_mode": "din"} |
| `110_ablate_c1_s2` | ablate | 0.60185 | 0.66797 | 0.53573 | -0.00211 | {"loss": "logloss", "seed": 2} |
| `034_ablate_c1_s2` | ablate | 0.60183 | 0.66766 | 0.53601 | -0.00156 | {"loss": "bpr_global", "seed": 2} |
| `000_fm_s1` | ablate | 0.60176 | 0.66739 | 0.53613 |  | {"aux_click_weight": 0.3, "cwm_weight": 0.2} |
| `119_ablate_c0_s2` | ablate | 0.60167 | 0.66745 | 0.53590 | -0.00228 | {"seed": 2, "seq_len": 20, "seq_mode": "pool"} |
| `122_ablate_c1_s2` | ablate | 0.60167 | 0.66745 | 0.53590 | -0.00228 | {"loss": "logloss", "seed": 2} |
| `090_ablate_c1_s2` | ablate | 0.60158 | 0.66729 | 0.53588 | -0.00237 | {"loss": "bpr_global", "seed": 2} |
| `000_fm_baseline` | draft | 0.60147 | 0.66713 | 0.53581 |  | {"aux_click_weight": 0.3, "cwm_weight": 0.2} |
| `001_fm_s2` | ablate | 0.60109 | 0.66706 | 0.53512 |  | {"aux_click_weight": 0.3, "cwm_weight": 0.2} |
| `008_draft` | draft | 0.57712 | 0.63148 | 0.52276 | -0.02432 | {"model_family": "gbm"} |

102 scored nodes. Full dump: [`trials.csv`](trials.csv).
