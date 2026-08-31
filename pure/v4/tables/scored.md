# Scored trials (valid primary, high → low)

Official FM on this scale is **0.60160**. Kit `evaluate.py` only.

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
| `105_ablate_c0_s0` | ablate | 0.63303 | 0.70817 | 0.55788 | 0.00131 | {"arch": "dcnv2", "seed": 0} |
| `108_ablate_c1_s0` | ablate | 0.63303 | 0.70817 | 0.55788 | 0.00131 | {"bpr_pairs_cap": 64, "seed": 0} |
| `132_ablate_c0_s1` | ablate | 0.63224 | 0.70750 | 0.55698 | -0.00161 | {"seed": 1, "use_hour": true} |
| `135_ablate_c1_s1` | ablate | 0.63224 | 0.70750 | 0.55698 | -0.00161 | {"bpr_decay_sample": true, "seed": 1} |
| `097_ablate_c0_s1` | ablate | 0.63217 | 0.70819 | 0.55616 | 0.00046 | {"seed": 1, "use_hour": true} |
| `100_ablate_c1_s1` | ablate | 0.63217 | 0.70819 | 0.55616 | 0.00046 | {"bpr_decay_sample": false, "seed": 1} |
| `087_capacity` | capacity | 0.63208 | 0.70802 | 0.55614 | 0.00636 | {"k": 8} |
| `088_ablate_c0_s0` | ablate | 0.63208 | 0.70802 | 0.55614 | 0.00636 | {"k": 8, "seed": 0} |
| `126_ablate_c1_s0` | ablate | 0.63061 | 0.70696 | 0.55426 | -0.00324 | {"loss": "logloss", "seed": 0} |
| `065_ensemble` | ensemble | 0.63059 | 0.70577 | 0.55542 | 0.00487 | ensemble:061_ablate_c0_s0,062_ablate_c0_s1,063_ablate_c0_s2 |
| `066_ensemble` | ensemble | 0.63059 | 0.70577 | 0.55542 | 0.00000 | ensemble:000_fm_baseline,000_fm_s1,001_fm_s2,009_ablate_c0_s0,010_ablate_c0_s… |
| `077_ensemble` | ensemble | 0.63059 | 0.70577 | 0.55542 | 0.00000 | ensemble:061_ablate_c0_s0,062_ablate_c0_s1,063_ablate_c0_s2,068_ablate_c0_s0,… |
| `084_ensemble` | ensemble | 0.63059 | 0.70577 | 0.55542 | 0.00000 | ensemble:080_ablate_c0_s0,081_ablate_c0_s1,082_ablate_c0_s2 |
| `085_ensemble` | ensemble | 0.63059 | 0.70577 | 0.55542 | 0.00000 | ensemble:061_ablate_c0_s0,062_ablate_c0_s1,063_ablate_c0_s2,068_ablate_c0_s0,… |
| `127_ablate_c1_s1` | ablate | 0.63025 | 0.70632 | 0.55418 | -0.00360 | {"loss": "logloss", "seed": 1} |
| `089_ablate_c0_s1` | ablate | 0.62970 | 0.70531 | 0.55409 | 0.00397 | {"k": 8, "seed": 1} |
| `095_time_shift` | time_shift | 0.62881 | 0.70408 | 0.55354 | -0.00291 | {"use_hour": true} |
| `096_ablate_c0_s0` | ablate | 0.62881 | 0.70408 | 0.55354 | -0.00291 | {"seed": 0, "use_hour": true} |
| `099_ablate_c1_s0` | ablate | 0.62881 | 0.70408 | 0.55354 | -0.00291 | {"bpr_decay_sample": false, "seed": 0} |
| `075_ensemble` | ensemble | 0.62809 | 0.70271 | 0.55346 | -0.00251 | ensemble:068_ablate_c0_s0,069_ablate_c0_s1,070_ablate_c0_s2 |
| `076_ensemble` | ensemble | 0.62809 | 0.70271 | 0.55346 | -0.00251 | ensemble:071_ablate_c1_s0,072_ablate_c1_s1,073_ablate_c1_s2 |
| `060_architecture` | architecture | 0.62733 | 0.70058 | 0.55408 | 0.00835 | {"arch": "deepfm"} |
| `061_ablate_c0_s0` | ablate | 0.62733 | 0.70058 | 0.55408 | 0.00835 | {"arch": "deepfm", "seed": 0} |
| `079_features` | features | 0.62733 | 0.70058 | 0.55408 | 0.00160 | {"use_itemcf": true} |
| `080_ablate_c0_s0` | ablate | 0.62733 | 0.70058 | 0.55408 | 0.00160 | {"seed": 0, "use_itemcf": true} |
| `070_ablate_c0_s2` | ablate | 0.62706 | 0.70151 | 0.55261 | 0.00133 | {"seed": 2, "seq_len": 100, "seq_mode": "din"} |
| `073_ablate_c1_s2` | ablate | 0.62706 | 0.70151 | 0.55261 | 0.00133 | {"bpr_pairs_cap": 64, "seed": 2} |
| `128_ablate_c1_s2` | ablate | 0.62696 | 0.70190 | 0.55201 | -0.00689 | {"loss": "logloss", "seed": 2} |
| `062_ablate_c0_s1` | ablate | 0.62576 | 0.69940 | 0.55213 | 0.00679 | {"arch": "deepfm", "seed": 1} |
| `081_ablate_c0_s1` | ablate | 0.62576 | 0.69940 | 0.55213 | 0.00004 | {"seed": 1, "use_itemcf": true} |
| `067_sequence` | sequence | 0.62565 | 0.69881 | 0.55248 | -0.00008 | {"seq_len": 100, "seq_mode": "din"} |
| `068_ablate_c0_s0` | ablate | 0.62565 | 0.69881 | 0.55248 | -0.00008 | {"seed": 0, "seq_len": 100, "seq_mode": "din"} |
| `071_ablate_c1_s0` | ablate | 0.62565 | 0.69881 | 0.55248 | -0.00008 | {"bpr_pairs_cap": 64, "seed": 0} |
| `098_ablate_c0_s2` | ablate | 0.62471 | 0.69805 | 0.55137 | -0.00700 | {"seed": 2, "use_hour": true} |
| `101_ablate_c1_s2` | ablate | 0.62471 | 0.69805 | 0.55137 | -0.00700 | {"bpr_decay_sample": false, "seed": 2} |
| `069_ablate_c0_s1` | ablate | 0.62455 | 0.69793 | 0.55117 | -0.00117 | {"seed": 1, "seq_len": 100, "seq_mode": "din"} |
| `072_ablate_c1_s1` | ablate | 0.62455 | 0.69793 | 0.55117 | -0.00117 | {"bpr_pairs_cap": 64, "seed": 1} |
| `063_ablate_c0_s2` | ablate | 0.62408 | 0.69766 | 0.55051 | 0.00511 | {"arch": "deepfm", "seed": 2} |
| `082_ablate_c0_s2` | ablate | 0.62408 | 0.69766 | 0.55051 | -0.00164 | {"seed": 2, "use_itemcf": true} |
| `149_capacity` | capacity | 0.62392 | 0.69614 | 0.55170 | -0.01113 | {"k": 16} |
| `086_multitask` | multitask | 0.62377 | 0.69565 | 0.55189 | -0.00196 | {"aux_click": true} |
| `047_ablate_c0_s2` | ablate | 0.62251 | 0.69607 | 0.54894 | 0.00578 | {"seed": 2, "use_beh_rank": true} |
| `050_ablate_c1_s2` | ablate | 0.62251 | 0.69607 | 0.54894 | 0.00578 | {"bpr_decay_sample": true, "seed": 2} |
| `058_ablate_c0_s2` | ablate | 0.62251 | 0.69607 | 0.54894 | 0.00353 | {"bpr_decay_sample": true, "seed": 2} |
| `052_ensemble` | ensemble | 0.62129 | 0.69424 | 0.54834 | 0.00210 | ensemble:045_ablate_c0_s0,046_ablate_c0_s1,047_ablate_c0_s2 |
| `053_ensemble` | ensemble | 0.62129 | 0.69424 | 0.54834 | 0.00000 | ensemble:048_ablate_c1_s0,049_ablate_c1_s1,050_ablate_c1_s2 |
| `054_ensemble` | ensemble | 0.62129 | 0.69424 | 0.54834 | 0.00000 | ensemble:045_ablate_c0_s0,046_ablate_c0_s1,047_ablate_c0_s2,048_ablate_c1_s0,… |
| `145_capacity` | capacity | 0.61945 | 0.69024 | 0.54866 | -0.01560 | {"k": 32} |
| `041_ensemble` | ensemble | 0.61940 | 0.69178 | 0.54702 | 0.00021 | ensemble:025_ablate_c0_s0,026_ablate_c0_s1,027_ablate_c0_s2,032_ablate_c0_s0,… |
| `039_ensemble` | ensemble | 0.61919 | 0.69137 | 0.54701 | 0.00036 | ensemble:032_ablate_c0_s0,033_ablate_c0_s1,034_ablate_c0_s2 |
| `040_ensemble` | ensemble | 0.61919 | 0.69137 | 0.54701 | 0.00000 | ensemble:025_ablate_c0_s0,026_ablate_c0_s1,027_ablate_c0_s2,032_ablate_c0_s0,… |
| `029_ensemble` | ensemble | 0.61883 | 0.69046 | 0.54720 | 0.00218 | ensemble:025_ablate_c0_s0,026_ablate_c0_s1,027_ablate_c0_s2 |
| `030_ensemble` | ensemble | 0.61883 | 0.69046 | 0.54720 | 0.00000 | ensemble:000_fm_baseline,000_fm_s1,001_fm_s2,009_ablate_c0_s0,010_ablate_c0_s… |
| `027_ablate_c0_s2` | ablate | 0.61819 | 0.69016 | 0.54621 | 0.01537 | {"seed": 2, "use_time_decay": true} |
| `120_ablate_c1_s2` | ablate | 0.61819 | 0.69016 | 0.54621 | -0.01566 | {"loss": "bpr_global", "seed": 2} |
| `046_ablate_c0_s1` | ablate | 0.61771 | 0.68995 | 0.54548 | 0.00098 | {"seed": 1, "use_beh_rank": true} |
| `049_ablate_c1_s1` | ablate | 0.61771 | 0.68995 | 0.54548 | 0.00098 | {"bpr_decay_sample": true, "seed": 1} |
| `057_ablate_c0_s1` | ablate | 0.61771 | 0.68995 | 0.54548 | -0.00126 | {"bpr_decay_sample": true, "seed": 1} |
| `034_ablate_c0_s2` | ablate | 0.61766 | 0.68928 | 0.54605 | 0.00101 | {"seed": 2, "wlr_play": true} |
| `037_ablate_c1_s2` | ablate | 0.61766 | 0.68928 | 0.54605 | 0.00101 | {"loss": "bpr_global", "seed": 2} |
| `031_watch_time` | watch_time | 0.61686 | 0.68771 | 0.54602 | 0.00021 | {"wlr_play": true} |
| `032_ablate_c0_s0` | ablate | 0.61686 | 0.68771 | 0.54602 | 0.00021 | {"seed": 0, "wlr_play": true} |
| `035_ablate_c1_s0` | ablate | 0.61686 | 0.68771 | 0.54602 | 0.00021 | {"loss": "bpr_global", "seed": 0} |
| `042_crossover` | features | 0.61686 | 0.68771 | 0.54602 | 0.00013 | {"use_itemcf": true} |
| `044_features` | features | 0.61671 | 0.68713 | 0.54630 | -0.00001 | {"use_beh_rank": true} |
| `045_ablate_c0_s0` | ablate | 0.61671 | 0.68713 | 0.54630 | -0.00001 | {"seed": 0, "use_beh_rank": true} |
| `048_ablate_c1_s0` | ablate | 0.61671 | 0.68713 | 0.54630 | -0.00001 | {"bpr_decay_sample": true, "seed": 0} |
| `055_crossover` | features | 0.61671 | 0.68713 | 0.54630 | -0.00226 | {"bpr_decay_sample": true} |
| `056_ablate_c0_s0` | ablate | 0.61671 | 0.68713 | 0.54630 | -0.00226 | {"bpr_decay_sample": true, "seed": 0} |
| `026_ablate_c0_s1` | ablate | 0.61629 | 0.68651 | 0.54608 | 0.01347 | {"seed": 1, "use_time_decay": true} |
| `119_ablate_c1_s1` | ablate | 0.61629 | 0.68651 | 0.54608 | -0.01755 | {"loss": "bpr_global", "seed": 1} |
| `033_ablate_c0_s1` | ablate | 0.61566 | 0.68673 | 0.54459 | -0.00099 | {"seed": 1, "wlr_play": true} |
| `036_ablate_c1_s1` | ablate | 0.61566 | 0.68673 | 0.54459 | -0.00099 | {"loss": "bpr_global", "seed": 1} |
| `024_features` | features | 0.61547 | 0.68530 | 0.54563 | 0.01265 | {"use_time_decay": true} |
| `025_ablate_c0_s0` | ablate | 0.61547 | 0.68530 | 0.54563 | 0.01265 | {"seed": 0, "use_time_decay": true} |
| `118_ablate_c1_s0` | ablate | 0.61547 | 0.68530 | 0.54563 | -0.01838 | {"loss": "bpr_global", "seed": 0} |
| `147_capacity` | capacity | 0.61147 | 0.68087 | 0.54207 | -0.02358 | {"k": 64} |
| `116_ablate_c0_s1` | ablate | 0.60835 | 0.67505 | 0.54164 | -0.02550 | {"seed": 1, "use_time_decay": true} |
| `117_ablate_c0_s2` | ablate | 0.60726 | 0.67380 | 0.54072 | -0.02659 | {"seed": 2, "use_time_decay": true} |
| `155_ablate_c0_s2` | ablate | 0.60617 | 0.67064 | 0.54169 | -0.02888 | {"model_family": "gbm", "seed": 2} |
| `154_ablate_c0_s1` | ablate | 0.60593 | 0.67031 | 0.54156 | -0.02912 | {"model_family": "gbm", "seed": 1} |
| `152_architecture` | architecture | 0.60584 | 0.67021 | 0.54147 | -0.02921 | {"model_family": "gbm"} |
| `153_ablate_c0_s0` | ablate | 0.60584 | 0.67021 | 0.54147 | -0.02921 | {"model_family": "gbm", "seed": 0} |
| `020_ensemble` | ensemble | 0.60441 | 0.67100 | 0.53782 | 0.00159 | ensemble:009_ablate_c0_s0,010_ablate_c0_s1,011_ablate_c0_s2 |
| `007_draft` | draft | 0.60392 | 0.67040 | 0.53743 | 0.00248 | {"loss": "bpr_global"} |
| `009_ablate_c0_s0` | ablate | 0.60392 | 0.67040 | 0.53743 | 0.00248 | {"loss": "bpr_global", "seed": 0} |
| `023_multitask` | multitask | 0.60356 | 0.67011 | 0.53702 | 0.00074 | {"aux_click": true} |
| `114_features` | features | 0.60306 | 0.66907 | 0.53705 | -0.03079 | {"use_time_decay": true} |
| `115_ablate_c0_s0` | ablate | 0.60306 | 0.66907 | 0.53705 | -0.03079 | {"seed": 0, "use_time_decay": true} |
| `010_ablate_c0_s1` | ablate | 0.60249 | 0.66865 | 0.53634 | 0.00105 | {"loss": "bpr_global", "seed": 1} |
| `011_ablate_c0_s2` | ablate | 0.60205 | 0.66797 | 0.53612 | 0.00061 | {"loss": "bpr_global", "seed": 2} |
| `021_ensemble` | ensemble | 0.60189 | 0.66766 | 0.53612 | -0.00252 | ensemble:000_fm_baseline,000_fm_s1,001_fm_s2 |
| `022_ensemble` | ensemble | 0.60189 | 0.66766 | 0.53612 | -0.00252 | ensemble:000_fm_baseline,000_fm_s1,001_fm_s2,009_ablate_c0_s0,010_ablate_c0_s… |
| `000_fm_s1` | ablate | 0.60176 | 0.66739 | 0.53613 |  | {"aux_click_weight": 0.3, "cwm_weight": 0.2} |
| `000_fm_baseline` | draft | 0.60147 | 0.66713 | 0.53581 |  | {"aux_click_weight": 0.3, "cwm_weight": 0.2} |
| `001_fm_s2` | ablate | 0.60109 | 0.66706 | 0.53512 |  | {"aux_click_weight": 0.3, "cwm_weight": 0.2} |
| `015_ablate_c0_s2` | ablate | 0.57813 | 0.63264 | 0.52362 | -0.02469 | {"model_family": "gbm", "seed": 2} |
| `018_ablate_c1_s2` | ablate | 0.57813 | 0.63264 | 0.52362 | -0.02469 | {"loss": "bpr_global", "seed": 2} |
| `014_ablate_c0_s1` | ablate | 0.57790 | 0.63234 | 0.52346 | -0.02492 | {"model_family": "gbm", "seed": 1} |
| `017_ablate_c1_s1` | ablate | 0.57790 | 0.63234 | 0.52346 | -0.02492 | {"loss": "bpr_global", "seed": 1} |
| `008_draft` | draft | 0.57712 | 0.63148 | 0.52276 | -0.02432 | {"model_family": "gbm"} |
| `013_ablate_c0_s0` | ablate | 0.57712 | 0.63148 | 0.52276 | -0.02570 | {"model_family": "gbm", "seed": 0} |
| `016_ablate_c1_s0` | ablate | 0.57712 | 0.63148 | 0.52276 | -0.02570 | {"loss": "bpr_global", "seed": 0} |
| `122_architecture` | architecture | 0.53574 | 0.57344 | 0.49805 | -0.09811 | {"model_family": "torch"} |
| `123_ablate_c0_s0` | ablate | 0.53574 | 0.57344 | 0.49805 | -0.09811 | {"model_family": "torch", "seed": 0} |
| `125_ablate_c0_s2` | ablate | 0.53560 | 0.57341 | 0.49780 | -0.09825 | {"model_family": "torch", "seed": 2} |
| `124_ablate_c0_s1` | ablate | 0.53258 | 0.56898 | 0.49618 | -0.10127 | {"model_family": "torch", "seed": 1} |

132 scored nodes. Full dump: [`trials.csv`](trials.csv).
