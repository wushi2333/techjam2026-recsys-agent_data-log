# Auto findings (not a to-do list)

Tagged measurements written by the harness from journals.
[measured-3seed] is fact; [measured-1seed] needs ablate; [diagnosis] is a direction.
Do not treat this file as a human trial agenda.

- [measured-3seed] incumbent 143_ensemble is_bag=True submit=0.63931 seed0=0.63558 member_mean=0.63505 screen_bar=0.63505
- [measured-3seed] 000_fm_baseline seed0=0.60147 mean=0.60144 patch={'aux_click_weight': 0.3, 'cwm_weight': 0.2}
- [measured-3seed] 009_ablate_c0_s0 seed0=0.60392 mean=0.60282 patch={'loss': 'bpr_global', 'seed': 0}
- [measured-3seed] 020_ensemble seed0=0.60441 mean=na patch=['009_ablate_c0_s0', '010_ablate_c0_s1', '011_ablate_c0_s2']
- [measured-3seed] 025_ablate_c0_s0 seed0=0.61547 mean=0.61665 patch={'use_time_decay': True, 'seed': 0}
- [measured-3seed] 029_ensemble seed0=0.61883 mean=na patch=['025_ablate_c0_s0', '026_ablate_c0_s1', '027_ablate_c0_s2']
- [measured-3seed] 039_ensemble seed0=0.61919 mean=na patch=['032_ablate_c0_s0', '033_ablate_c0_s1', '034_ablate_c0_s2']
- [measured-3seed] 052_ensemble seed0=0.62129 mean=na patch=['045_ablate_c0_s0', '046_ablate_c0_s1', '047_ablate_c0_s2']
- [measured-3seed] 053_ensemble seed0=0.62129 mean=na patch=['048_ablate_c1_s0', '049_ablate_c1_s1', '050_ablate_c1_s2']
- [measured-3seed] 061_ablate_c0_s0 seed0=0.62733 mean=0.62573 patch={'arch': 'deepfm', 'seed': 0}
- [measured-3seed] 065_ensemble seed0=0.63059 mean=na patch=['061_ablate_c0_s0', '062_ablate_c0_s1', '063_ablate_c0_s2']
- [measured-3seed] 084_ensemble seed0=0.63059 mean=na patch=['080_ablate_c0_s0', '081_ablate_c0_s1', '082_ablate_c0_s2']
- [measured-3seed] 088_ablate_c0_s0 seed0=0.63208 mean=0.63172 patch={'k': 8, 'seed': 0}
- [measured-3seed] 092_ensemble seed0=0.63335 mean=na patch=['088_ablate_c0_s0', '089_ablate_c0_s1', '090_ablate_c0_s2']
- [measured-3seed] 105_ablate_c0_s0 seed0=0.63303 mean=0.63385 patch={'arch': 'dcnv2', 'seed': 0}
- [measured-3seed] 112_ensemble seed0=0.63692 mean=na patch=['105_ablate_c0_s0', '106_ablate_c0_s1', '107_ablate_c0_s2']
- [measured-3seed] 143_ensemble seed0=0.63931 mean=na patch=['139_ablate_c0_s0', '140_ablate_c0_s1', '141_ablate_c0_s2']
- [measured-1seed] 008_draft parent=(root) scale=pure {'model_family': 'gbm'} dP=-0.02432 CI_hi=-0.02093  # draft 1-seed
- [measured-1seed] 031_watch_time parent=029_ensemble scale=pure {'wlr_play': True} dP=0.00021 CI_hi=-0.00026  # 1-seed on this parent, not 3-seed
- [measured-1seed] 042_crossover parent=039_ensemble scale=pure {'use_itemcf': True} dP=0.00013 CI_hi=-0.00103  # 1-seed on this parent, not 3-seed
- [measured-1seed] 044_features parent=039_ensemble scale=pure {'use_beh_rank': True} dP=-0.00001 CI_hi=-0.00017  # 1-seed on this parent, not 3-seed
- [measured-1seed] 055_crossover parent=052_ensemble scale=pure {'bpr_decay_sample': True} dP=-0.00226 CI_hi=-0.00317  # 1-seed on this parent, not 3-seed
- [measured-1seed] 067_sequence parent=065_ensemble scale=pure {'seq_len': 100, 'seq_mode': 'din'} dP=-0.00008 CI_hi=-0.00329  # 1-seed on this parent, not 3-seed
- [measured-1seed] 086_multitask parent=065_ensemble scale=pure {'aux_click': True} dP=-0.00196 CI_hi=-0.00536  # 1-seed on this parent, not 3-seed
- [measured-1seed] 095_time_shift parent=092_ensemble scale=pure {'use_hour': True} dP=-0.00291 CI_hi=-0.00323  # 1-seed on this parent, not 3-seed
- [measured-1seed] 114_features parent=000_fm_baseline scale=pure {'use_time_decay': True} dP=-0.03079 CI_hi=-0.03159  # 1-seed on this parent, not 3-seed
- [measured-1seed] 122_architecture parent=112_ensemble scale=pure {'model_family': 'torch'} dP=-0.09811 CI_hi=-0.09756  # 1-seed on this parent, not 3-seed
- [measured-1seed] 145_capacity parent=143_ensemble scale=pure {'k': 32} dP=-0.01560 CI_hi=-0.01759  # 1-seed on this parent, not 3-seed
- [measured-1seed] 146_loss parent=143_ensemble scale=pure {'bpr_pairs_cap': 64} dP=0.00053 CI_hi=-0.00262  # 1-seed on this parent, not 3-seed
- [measured-1seed] 147_capacity parent=143_ensemble scale=pure {'k': 64} dP=-0.02358 CI_hi=-0.02551  # 1-seed on this parent, not 3-seed
- [measured-1seed] 149_capacity parent=143_ensemble scale=pure {'k': 16} dP=-0.01113 CI_hi=-0.01353  # 1-seed on this parent, not 3-seed
- [measured-1seed] 150_loss parent=143_ensemble scale=pure {'bpr_pairs_cap': 16} dP=0.00053 CI_hi=-0.00262  # 1-seed on this parent, not 3-seed
- [diagnosis] pred_calibration: 14/101 expected_delta within CI, mean_bias=+0.00832 (over-optimistic)
