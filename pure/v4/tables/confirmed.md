# Confirmed identities

- `000_fm_baseline` primary=0.60147 patch={"aux_click_weight": 0.3, "cwm_weight": 0.2}
- `009_ablate_c0_s0` primary=0.60392 patch={"loss": "bpr_global", "seed": 0}
- `020_ensemble` primary=0.60441 patch=ensemble:009_ablate_c0_s0,010_ablate_c0_s1,011_ablate_c0_s2
- `025_ablate_c0_s0` primary=0.61547 patch={"seed": 0, "use_time_decay": true}
- `029_ensemble` primary=0.61883 patch=ensemble:025_ablate_c0_s0,026_ablate_c0_s1,027_ablate_c0_s2
- `039_ensemble` primary=0.61919 patch=ensemble:032_ablate_c0_s0,033_ablate_c0_s1,034_ablate_c0_s2
- `052_ensemble` primary=0.62129 patch=ensemble:045_ablate_c0_s0,046_ablate_c0_s1,047_ablate_c0_s2
- `053_ensemble` primary=0.62129 patch=ensemble:048_ablate_c1_s0,049_ablate_c1_s1,050_ablate_c1_s2
- `061_ablate_c0_s0` primary=0.62733 patch={"arch": "deepfm", "seed": 0}
- `065_ensemble` primary=0.63059 patch=ensemble:061_ablate_c0_s0,062_ablate_c0_s1,063_ablate_c0_s2
- `084_ensemble` primary=0.63059 patch=ensemble:080_ablate_c0_s0,081_ablate_c0_s1,082_ablate_c0_s2
- `088_ablate_c0_s0` primary=0.63208 patch={"k": 8, "seed": 0}
- `092_ensemble` primary=0.63335 patch=ensemble:088_ablate_c0_s0,089_ablate_c0_s1,090_ablate_c0_s2
- `105_ablate_c0_s0` primary=0.63303 patch={"arch": "dcnv2", "seed": 0}
- `112_ensemble` primary=0.63692 patch=ensemble:105_ablate_c0_s0,106_ablate_c0_s1,107_ablate_c0_s2
- `143_ensemble` primary=0.63931 patch=ensemble:139_ablate_c0_s0,140_ablate_c0_s1,141_ablate_c0_s2
