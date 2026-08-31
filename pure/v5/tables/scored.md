# Scored trials (valid primary, high → low)

Official FM on this scale is **0.60160**. Kit `evaluate.py` only.

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
| `131_ablate_c0_s1` | ablate | 0.60399 | 0.67033 | 0.53764 | 0.00004 | {"seed": 1, "seq_len": 50, "seq_mode": "din"} |
| `100_ablate_c0_s2` | ablate | 0.60398 | 0.67037 | 0.53759 | 0.00012 | {"seed": 2, "seq_len": 50, "seq_mode": "din"} |
| `103_ablate_c1_s2` | ablate | 0.60398 | 0.67037 | 0.53759 | 0.00012 | {"arch": "deepfm", "seed": 2} |
| `132_ablate_c0_s2` | ablate | 0.60398 | 0.67037 | 0.53759 | 0.00003 | {"seed": 2, "seq_len": 50, "seq_mode": "din"} |
| `107_sequence` | sequence | 0.60396 | 0.67006 | 0.53786 | 0.00001 | {"seq_len": 100, "seq_mode": "pool"} |
| `108_ablate_c0_s0` | ablate | 0.60396 | 0.67006 | 0.53786 | 0.00001 | {"seed": 0, "seq_len": 100, "seq_mode": "pool"} |
| `142_ablate_c1_s0` | ablate | 0.60396 | 0.67045 | 0.53746 | 0.00001 | {"loss": "bpr_global", "seed": 0} |
| `056_sequence` | sequence | 0.60394 | 0.66988 | 0.53800 | 0.00008 | {"seq_len": 20, "seq_mode": "pool"} |
| `057_ablate_c0_s0` | ablate | 0.60394 | 0.66988 | 0.53800 | 0.00008 | {"seed": 0, "seq_len": 20, "seq_mode": "pool"} |
| `077_sequence` | sequence | 0.60394 | 0.66996 | 0.53792 | 0.00008 | {"seq_len": 20, "seq_mode": "din"} |
| `078_ablate_c0_s0` | ablate | 0.60394 | 0.66996 | 0.53792 | 0.00008 | {"seed": 0, "seq_len": 20, "seq_mode": "din"} |
| `052_ensemble` | ensemble | 0.60394 | 0.67023 | 0.53765 | 0.00008 | ensemble:045_ablate_c0_s0,046_ablate_c0_s1,047_ablate_c0_s2 |
| `030_loss` | loss | 0.60392 | 0.67040 | 0.53743 | 0.00006 | {"loss": "bpr_global"} |
| `151_ablate_c1_s0` | ablate | 0.60391 | 0.67035 | 0.53747 | -0.00004 | {"loss": "bpr_global", "seed": 0} |
| `091_ablate_c1_s0` | ablate | 0.60390 | 0.67023 | 0.53757 | 0.00004 | {"loss": "bpr_global", "seed": 0} |
| `090_ablate_c0_s2` | ablate | 0.60389 | 0.67023 | 0.53756 | 0.00003 | {"seed": 2, "seq_len": 50, "seq_mode": "pool"} |
| `087_sequence` | sequence | 0.60389 | 0.66995 | 0.53783 | 0.00003 | {"seq_len": 50, "seq_mode": "pool"} |
| `088_ablate_c0_s0` | ablate | 0.60389 | 0.66995 | 0.53783 | 0.00003 | {"seed": 0, "seq_len": 50, "seq_mode": "pool"} |
| `109_ablate_c0_s1` | ablate | 0.60389 | 0.67008 | 0.53770 | -0.00006 | {"seed": 1, "seq_len": 100, "seq_mode": "pool"} |
| `097_sequence` | sequence | 0.60388 | 0.66993 | 0.53783 | 0.00002 | {"seq_len": 50, "seq_mode": "din"} |
| `098_ablate_c0_s0` | ablate | 0.60388 | 0.66993 | 0.53783 | 0.00002 | {"seed": 0, "seq_len": 50, "seq_mode": "din"} |
| `101_ablate_c1_s0` | ablate | 0.60388 | 0.66993 | 0.53783 | 0.00002 | {"arch": "deepfm", "seed": 0} |
| `130_ablate_c0_s0` | ablate | 0.60388 | 0.66993 | 0.53783 | -0.00007 | {"seed": 0, "seq_len": 50, "seq_mode": "din"} |
| `007_draft` | draft | 0.60383 | 0.66997 | 0.53769 | 0.00239 | {"arch": "deepfm"} |
| `009_ablate_c0_s0` | ablate | 0.60383 | 0.66997 | 0.53769 | 0.00239 | {"arch": "deepfm", "seed": 0} |
| `024_ablate_c1_s0` | ablate | 0.60383 | 0.66997 | 0.53769 | -0.00003 | {"arch": "deepfm", "seed": 0} |
| `044_sequence` | sequence | 0.60382 | 0.66993 | 0.53770 | -0.00004 | {"seq_len": 10, "seq_mode": "din"} |
| `045_ablate_c0_s0` | ablate | 0.60382 | 0.66993 | 0.53770 | -0.00004 | {"seed": 0, "seq_len": 10, "seq_mode": "din"} |
| `089_ablate_c0_s1` | ablate | 0.60379 | 0.66997 | 0.53761 | -0.00007 | {"seed": 1, "seq_len": 50, "seq_mode": "pool"} |
| `022_ablate_c0_s1` | ablate | 0.60374 | 0.67032 | 0.53715 | -0.00013 | {"arch": "dcnv2", "seed": 1} |
| `133_ablate_c1_s0` | ablate | 0.60372 | 0.67009 | 0.53735 | -0.00023 | {"loss": "bpr_global", "seed": 0} |
| `060_ablate_c1_s0` | ablate | 0.60372 | 0.67053 | 0.53690 | -0.00014 | {"loss": "bpr_global", "seed": 0} |
| `081_ablate_c1_s0` | ablate | 0.60371 | 0.67024 | 0.53717 | -0.00016 | {"loss": "bpr_global", "seed": 0} |
| `059_ablate_c0_s2` | ablate | 0.60370 | 0.66995 | 0.53745 | -0.00016 | {"seed": 2, "seq_len": 20, "seq_mode": "pool"} |
| `023_ablate_c0_s2` | ablate | 0.60369 | 0.67002 | 0.53736 | -0.00017 | {"arch": "dcnv2", "seed": 2} |
| `010_ablate_c0_s1` | ablate | 0.60369 | 0.67011 | 0.53726 | 0.00224 | {"arch": "deepfm", "seed": 1} |
| `025_ablate_c1_s1` | ablate | 0.60369 | 0.67011 | 0.53726 | -0.00018 | {"arch": "deepfm", "seed": 1} |
| `033_sequence` | sequence | 0.60368 | 0.66969 | 0.53766 | -0.00019 | {"seq_len": 10, "seq_mode": "pool"} |
| `034_ablate_c0_s0` | ablate | 0.60368 | 0.66969 | 0.53766 | -0.00019 | {"seed": 0, "seq_len": 10, "seq_mode": "pool"} |
| `012_ablate_c1_s0` | ablate | 0.60362 | 0.66992 | 0.53733 | 0.00218 | {"loss": "bpr_global", "seed": 0} |
| `032_loss` | loss | 0.60362 | 0.66992 | 0.53733 | -0.00024 | {"loss": "bpr_global"} |
| `028_ensemble` | ensemble | 0.60361 | 0.67007 | 0.53715 | -0.00025 | ensemble:021_ablate_c0_s0,022_ablate_c0_s1,023_ablate_c0_s2 |
| `112_ablate_c1_s1` | ablate | 0.60360 | 0.67022 | 0.53697 | -0.00035 | {"loss": "bpr_global", "seed": 1} |
| `013_ablate_c1_s1` | ablate | 0.60356 | 0.67050 | 0.53663 | 0.00212 | {"loss": "bpr_global", "seed": 1} |
| `079_ablate_c0_s1` | ablate | 0.60355 | 0.66983 | 0.53727 | -0.00031 | {"seed": 1, "seq_len": 20, "seq_mode": "din"} |
| `122_ablate_c0_s1` | ablate | 0.60353 | 0.67011 | 0.53695 | -0.00042 | {"arch": "dcnv2", "seed": 1} |
| `111_ablate_c1_s0` | ablate | 0.60352 | 0.66969 | 0.53734 | -0.00043 | {"loss": "bpr_global", "seed": 0} |
| `058_ablate_c0_s1` | ablate | 0.60351 | 0.66980 | 0.53722 | -0.00035 | {"seed": 1, "seq_len": 20, "seq_mode": "pool"} |
| `092_ablate_c1_s1` | ablate | 0.60350 | 0.67020 | 0.53681 | -0.00036 | {"loss": "bpr_global", "seed": 1} |
| `123_ablate_c0_s2` | ablate | 0.60350 | 0.67005 | 0.53694 | -0.00045 | {"arch": "dcnv2", "seed": 2} |
| `080_ablate_c0_s2` | ablate | 0.60348 | 0.66964 | 0.53732 | -0.00038 | {"seed": 2, "seq_len": 20, "seq_mode": "din"} |
| `036_ablate_c0_s2` | ablate | 0.60343 | 0.66965 | 0.53721 | -0.00043 | {"seed": 2, "seq_len": 10, "seq_mode": "pool"} |
| `120_architecture` | architecture | 0.60342 | 0.66980 | 0.53703 | -0.00053 | {"arch": "dcnv2"} |
| `121_ablate_c0_s0` | ablate | 0.60342 | 0.66980 | 0.53703 | -0.00053 | {"arch": "dcnv2", "seed": 0} |
| `134_ablate_c1_s1` | ablate | 0.60340 | 0.67005 | 0.53676 | -0.00054 | {"loss": "bpr_global", "seed": 1} |
| `047_ablate_c0_s2` | ablate | 0.60337 | 0.66957 | 0.53718 | -0.00049 | {"seed": 2, "seq_len": 10, "seq_mode": "din"} |
| `035_ablate_c0_s1` | ablate | 0.60336 | 0.66927 | 0.53745 | -0.00050 | {"seed": 1, "seq_len": 10, "seq_mode": "pool"} |
| `037_ablate_c1_s0` | ablate | 0.60328 | 0.66946 | 0.53709 | -0.00059 | {"loss": "bpr_global", "seed": 0} |
| `038_ablate_c1_s1` | ablate | 0.60324 | 0.66949 | 0.53699 | -0.00062 | {"loss": "bpr_global", "seed": 1} |
| `125_ablate_c1_s1` | ablate | 0.60324 | 0.66945 | 0.53702 | -0.00071 | {"loss": "bpr_global", "seed": 1} |
| `113_ablate_c1_s2` | ablate | 0.60321 | 0.67004 | 0.53639 | -0.00073 | {"loss": "bpr_global", "seed": 2} |
| `046_ablate_c0_s1` | ablate | 0.60321 | 0.66926 | 0.53716 | -0.00065 | {"seed": 1, "seq_len": 10, "seq_mode": "din"} |
| `049_ablate_c1_s1` | ablate | 0.60318 | 0.66943 | 0.53692 | -0.00068 | {"loss": "bpr_global", "seed": 1} |
| `082_ablate_c1_s1` | ablate | 0.60318 | 0.66950 | 0.53685 | -0.00069 | {"loss": "bpr_global", "seed": 1} |
| `048_ablate_c1_s0` | ablate | 0.60316 | 0.66926 | 0.53705 | -0.00071 | {"loss": "bpr_global", "seed": 0} |
| `067_sequence` | sequence | 0.60311 | 0.66938 | 0.53684 | -0.00075 | {"seq_len": 100, "seq_mode": "pool"} |
| `068_ablate_c0_s0` | ablate | 0.60311 | 0.66938 | 0.53684 | -0.00075 | {"seed": 0, "seq_len": 100, "seq_mode": "pool"} |
| `083_ablate_c1_s2` | ablate | 0.60310 | 0.66980 | 0.53640 | -0.00076 | {"loss": "bpr_global", "seed": 2} |
| `061_ablate_c1_s1` | ablate | 0.60300 | 0.66920 | 0.53680 | -0.00086 | {"loss": "bpr_global", "seed": 1} |
| `135_ablate_c1_s2` | ablate | 0.60300 | 0.66965 | 0.53635 | -0.00095 | {"loss": "bpr_global", "seed": 2} |
| `014_ablate_c1_s2` | ablate | 0.60300 | 0.66959 | 0.53640 | 0.00156 | {"loss": "bpr_global", "seed": 2} |
| `062_ablate_c1_s2` | ablate | 0.60299 | 0.66955 | 0.53642 | -0.00088 | {"loss": "bpr_global", "seed": 2} |
| `124_ablate_c1_s0` | ablate | 0.60294 | 0.66903 | 0.53685 | -0.00101 | {"loss": "bpr_global", "seed": 0} |
| `116_regularization` | regularization | 0.60293 | 0.66900 | 0.53687 | -0.00102 | {"l2": 1e-05} |
| `117_regularization` | regularization | 0.60293 | 0.66911 | 0.53675 | -0.00102 | {"l2": 5e-06} |
| `020_architecture` | architecture | 0.60289 | 0.66910 | 0.53669 | -0.00097 | {"arch": "dcnv2"} |
| `021_ablate_c0_s0` | ablate | 0.60289 | 0.66910 | 0.53669 | -0.00097 | {"arch": "dcnv2", "seed": 0} |
| `093_ablate_c1_s2` | ablate | 0.60289 | 0.66945 | 0.53633 | -0.00097 | {"loss": "bpr_global", "seed": 2} |
| `119_capacity` | capacity | 0.60286 | 0.66879 | 0.53692 | -0.00109 | {"k": 8} |
| `147_sequence` | sequence | 0.60280 | 0.66864 | 0.53695 | -0.00115 | {"seq_len": 20, "seq_mode": "pool"} |
| `148_ablate_c0_s0` | ablate | 0.60280 | 0.66864 | 0.53695 | -0.00115 | {"seed": 0, "seq_len": 20, "seq_mode": "pool"} |
| `050_ablate_c1_s2` | ablate | 0.60271 | 0.66850 | 0.53691 | -0.00116 | {"loss": "bpr_global", "seed": 2} |
| `075_ensemble` | ensemble | 0.60266 | 0.66896 | 0.53637 | -0.00120 | ensemble:068_ablate_c0_s0,069_ablate_c0_s1,070_ablate_c0_s2 |
| `152_ablate_c1_s1` | ablate | 0.60264 | 0.66853 | 0.53676 | -0.00131 | {"loss": "bpr_global", "seed": 1} |
| `143_ablate_c1_s1` | ablate | 0.60263 | 0.66852 | 0.53673 | -0.00132 | {"loss": "bpr_global", "seed": 1} |
| `138_sequence` | sequence | 0.60257 | 0.66874 | 0.53641 | -0.00138 | {"seq_len": 20, "seq_mode": "din"} |
| `139_ablate_c0_s0` | ablate | 0.60257 | 0.66874 | 0.53641 | -0.00138 | {"seed": 0, "seq_len": 20, "seq_mode": "din"} |
| `140_ablate_c0_s1` | ablate | 0.60253 | 0.66860 | 0.53647 | -0.00142 | {"seed": 1, "seq_len": 20, "seq_mode": "din"} |
| `146_regularization` | regularization | 0.60247 | 0.66817 | 0.53676 | -0.00148 | {"l2": 0.0001} |
| `153_ablate_c1_s2` | ablate | 0.60246 | 0.66869 | 0.53622 | -0.00149 | {"loss": "bpr_global", "seed": 2} |
| `039_ablate_c1_s2` | ablate | 0.60241 | 0.66820 | 0.53662 | -0.00145 | {"loss": "bpr_global", "seed": 2} |
| `144_ablate_c1_s2` | ablate | 0.60238 | 0.66859 | 0.53617 | -0.00157 | {"loss": "bpr_global", "seed": 2} |
| `149_ablate_c0_s1` | ablate | 0.60229 | 0.66834 | 0.53624 | -0.00166 | {"seed": 1, "seq_len": 20, "seq_mode": "pool"} |
| `070_ablate_c0_s2` | ablate | 0.60213 | 0.66783 | 0.53644 | -0.00173 | {"seed": 2, "seq_len": 100, "seq_mode": "pool"} |
| `069_ablate_c0_s1` | ablate | 0.60209 | 0.66815 | 0.53603 | -0.00177 | {"seed": 1, "seq_len": 100, "seq_mode": "pool"} |
| `156_sequence` | sequence | 0.60207 | 0.66790 | 0.53624 | -0.00188 | {"seq_len": 10, "seq_mode": "din"} |
| `072_ablate_c1_s1` | ablate | 0.60205 | 0.66782 | 0.53628 | -0.00182 | {"loss": "bpr_global", "seed": 1} |
| `073_ablate_c1_s2` | ablate | 0.60200 | 0.66803 | 0.53597 | -0.00186 | {"loss": "bpr_global", "seed": 2} |
| `141_ablate_c0_s2` | ablate | 0.60191 | 0.66788 | 0.53594 | -0.00204 | {"seed": 2, "seq_len": 20, "seq_mode": "din"} |
| `000_fm_s1` | ablate | 0.60176 | 0.66739 | 0.53613 |  | {"aux_click_weight": 0.3, "cwm_weight": 0.2} |
| `150_ablate_c0_s2` | ablate | 0.60167 | 0.66745 | 0.53590 | -0.00228 | {"seed": 2, "seq_len": 20, "seq_mode": "pool"} |
| `000_fm_baseline` | draft | 0.60147 | 0.66713 | 0.53581 |  | {"aux_click_weight": 0.3, "cwm_weight": 0.2} |
| `126_ablate_c1_s2` | ablate | 0.60147 | 0.66702 | 0.53592 | -0.00248 | {"loss": "bpr_global", "seed": 2} |
| `001_fm_s2` | ablate | 0.60109 | 0.66706 | 0.53512 |  | {"aux_click_weight": 0.3, "cwm_weight": 0.2} |
| `055_capacity` | capacity | 0.60003 | 0.66572 | 0.53433 | -0.00384 | {"k": 8} |
| `008_draft` | draft | 0.57712 | 0.63148 | 0.52276 | -0.02432 | {"model_family": "gbm"} |

131 scored nodes. Full dump: [`trials.csv`](trials.csv).
