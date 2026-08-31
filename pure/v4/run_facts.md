## run_facts (auto-written from journal; not human agenda)
env: cuda=1 vram_gb=8.0 torch=1 lightgbm=1
job_data_scale=pure  # pinned at launch; this run's task instance, not a search arm
legal_families=fm,gbm,torch
legal_scales=pure,1k
datasets:
  pure present published_rows=1436609 log_bytes=105726357
  1k present published_rows=11713045 log_bytes=865973843
  27k absent
env_facts: IDs are re-indexed across Pure/1K/27K so they are not the same task; do not compare 1K primary to Pure FM 0.6016; contest hidden test is Pure.

vs_object=0.63505  # screen bar: member 3-seed mean if bagged, else confirmed_mean/seed0
incumbent=143_ensemble is_bag=True submit_primary=0.63931 seed0_primary=0.63558 confirmed_mean=na member_mean=0.63505 weak=False se_val=0.00073
# submit_primary is bag if is_bag else the node; screen vs vs_object, not submit_primary
incumbent_config={'k': 8, 'lr': 0.001, 'l2': 1e-06, 'epochs': 40, 'batch': 8192, 'patience': 4, 'seed': 0, 'loss': 'bpr_global', 'listwise_gain': 'uniform', 'bpr_pairs_cap': 32, 'train_tail_stop': False, 'model_family': 'fm', 'seq_len': 0, 'seq_mode': 'none', 'use_hour': False, 'use_itemcf': True, 'use_beh_cross': False, 'use_beh_rank': True, 'use_time_decay': True, 'wlr_play': True, 'bpr_decay_sample': True, 'aux_click': True, 'aux_click_weight': 0.3, 'cwm_censor': False, 'cwm_weight': 0.2, 'cwm_head': 'independent', 'arch': 'dcnv2', 'gbm_leaves': 31, 'gbm_rounds': 80, 'gbm_min_data': 20, 'gbm_feat_frac': 1.0, 'gbm_bag_frac': 1.0, 'gbm_lr': 0.05, 'gbm_cat': 'lowcard', 'smoke': False, 'max_train_rows': None, 'eval_split': 'valid', 'finalize': False, 'infer_split': 'valid', 'data_scale': 'pure'}

legal_untried (merged with incumbent; pick one atomic patch from these):
- loss: {'bpr_decay_sample': True}
- loss: {'loss': 'bpr_global'}
- features: {'use_itemcf': True}
- features: {'use_beh_rank': True}
- features: {'use_time_decay': True}
- watch_time: {'wlr_play': True}
- time_shift: {'use_hour': True}
- multitask: {'aux_click': True}
- sequence: {'seq_len': 100, 'seq_mode': 'din'}
- sequence: {'seq_len': 10, 'seq_mode': 'pool'}
- sequence: {'seq_len': 10, 'seq_mode': 'din'}
- sequence: {'seq_len': 20, 'seq_mode': 'pool'}
- … 11 more

eda=pair_cover=0.016 new_video=0.001 new_user=0.019 pos_train=0.337 pos_valid=0.313 valid_p50=4 valid_p90=12 train_p50=31 train_p90=97 train_mean=43.5 valid_mean=5.6 rows_per_user train/valid=7.8x single_imp=0.175 pos_drift=0.0059

confirmed:
- 000_fm_baseline seed0=0.60147 mean=0.60144 patch=None
- 009_ablate_c0_s0 seed0=0.60392 mean=0.60282 patch={'loss': 'bpr_global'}
- 020_ensemble seed0=0.60441 mean=na patch=None
- 025_ablate_c0_s0 seed0=0.61547 mean=0.61665 patch={'use_time_decay': True}
- 029_ensemble seed0=0.61883 mean=na patch=None
- 039_ensemble seed0=0.61919 mean=na patch=None
- 052_ensemble seed0=0.62129 mean=na patch=None
- 053_ensemble seed0=0.62129 mean=na patch=None
- 061_ablate_c0_s0 seed0=0.62733 mean=0.62573 patch={'arch': 'deepfm'}
- 065_ensemble seed0=0.63059 mean=na patch=None
- 084_ensemble seed0=0.63059 mean=na patch=None
- 088_ablate_c0_s0 seed0=0.63208 mean=0.63172 patch={'k': 8}
- 092_ensemble seed0=0.63335 mean=na patch=None
- 105_ablate_c0_s0 seed0=0.63303 mean=0.63385 patch={'arch': 'dcnv2'}
- 112_ensemble seed0=0.63692 mean=na patch=None
- 143_ensemble seed0=0.63931 mean=na patch=None

last_ablate=156_ablate vs_mean=0.63505
  c0 mean=0.60598 n_pos_vs_mean=0/3 std=0.00014 patch={'model_family': 'gbm', 'seed': 0}

screens (vs_object, not a promotion):
- 095_time_shift fail {'use_hour': True} primary=0.62881 dP=-0.00291 dGAUC=-0.00383 dNDCG=-0.00286 se_val=0.00066 tSplit=0.00099 dP_ref=screen_bar CI_ref=incumbent_scores top1=0.83359 itemcf_alpha=0.0
- 104_architecture fail {'arch': 'dcnv2'} primary=0.63303 dP=0.00131 dGAUC=0.00026 dNDCG=0.00148 se_val=0.00095 tSplit=0.00302 dP_ref=screen_bar CI_ref=incumbent_scores top1=0.75347 itemcf_alpha=0.0
- 114_features fail {'use_time_decay': True} primary=0.60306 dP=-0.03079 dGAUC=-0.04012 dNDCG=-0.02317 se_val=0.00120 tSplit=0.00517 dP_ref=screen_bar CI_ref=incumbent_scores top1=0.59160
- 122_architecture fail {'model_family': 'torch'} primary=0.53574 dP=-0.09811 dGAUC=-0.13575 dNDCG=-0.06218 se_val=0.00202 tSplit=0.00879 dP_ref=screen_bar CI_ref=incumbent_scores top1=0.30964 itemcf_alpha=2.0
- 130_time_shift pass {'use_hour': True} primary=0.63508 dP=0.00123 dGAUC=0.00166 dNDCG=-0.00091 se_val=0.00077 tSplit=0.00030 dP_ref=screen_bar CI_ref=incumbent_scores top1=0.80802 itemcf_alpha=0.0
- 138_multitask pass {'aux_click': True} primary=0.63558 dP=0.00173 dGAUC=0.00356 dNDCG=-0.00182 se_val=0.00070 tSplit=0.00100 dP_ref=screen_bar CI_ref=incumbent_scores top1=0.82362 itemcf_alpha=0.0
- 145_capacity fail {'k': 32} primary=0.61945 dP=-0.01560 dGAUC=-0.02120 dNDCG=-0.01310 se_val=0.00119 tSplit=0.00154 dP_ref=screen_bar CI_ref=incumbent_scores top1=0.66268 itemcf_alpha=0.0
- 146_loss fail {'bpr_pairs_cap': 64} primary=0.63558 dP=0.00053 dGAUC=0.00132 dNDCG=-0.00335 se_val=0.00059 tSplit=0.00135 dP_ref=screen_bar CI_ref=incumbent_scores top1=0.87438 itemcf_alpha=0.0
- 147_capacity fail {'k': 64} primary=0.61147 dP=-0.02358 dGAUC=-0.03056 dNDCG=-0.01970 se_val=0.00120 tSplit=0.00350 dP_ref=screen_bar CI_ref=incumbent_scores top1=0.64594 itemcf_alpha=0.0
- 149_capacity fail {'k': 16} primary=0.62392 dP=-0.01113 dGAUC=-0.01529 dNDCG=-0.01006 se_val=0.00093 tSplit=0.00220 dP_ref=screen_bar CI_ref=incumbent_scores top1=0.73781 itemcf_alpha=0.0
- 150_loss fail {'bpr_pairs_cap': 16} primary=0.63558 dP=0.00053 dGAUC=0.00132 dNDCG=-0.00335 se_val=0.00059 tSplit=0.00135 dP_ref=screen_bar CI_ref=incumbent_scores top1=0.87438 itemcf_alpha=0.0
- 152_architecture fail {'model_family': 'gbm'} primary=0.60584 dP=-0.02921 dGAUC=-0.04122 dNDCG=-0.02030 se_val=0.00166 tSplit=0.00169 dP_ref=screen_bar CI_ref=incumbent_scores top1=0.40482 itemcf_alpha=0.0

timeouts=(none)

falsified (CI high < 0, 1-seed screen, not 3-seed):
- 114_features parent=000_fm_baseline {'use_time_decay': True} dP=-0.03079 CI=[-0.03623,-0.03159]  # 1-seed on this parent; a new incumbent identity may retry
- 122_architecture parent=112_ensemble {'model_family': 'torch'} dP=-0.09811 CI=[-0.10532,-0.09756]  # 1-seed on this parent; a new incumbent identity may retry
- 145_capacity parent=143_ensemble {'k': 32} dP=-0.01560 CI=[-0.02213,-0.01759]  # 1-seed on this parent; a new incumbent identity may retry
- 146_loss parent=143_ensemble {'bpr_pairs_cap': 64} dP=0.00053 CI=[-0.00488,-0.00262]  # 1-seed on this parent; a new incumbent identity may retry
- 147_capacity parent=143_ensemble {'k': 64} dP=-0.02358 CI=[-0.03038,-0.02551]  # 1-seed on this parent; a new incumbent identity may retry
- 149_capacity parent=143_ensemble {'k': 16} dP=-0.01113 CI=[-0.01710,-0.01353]  # 1-seed on this parent; a new incumbent identity may retry
- 150_loss parent=143_ensemble {'bpr_pairs_cap': 16} dP=0.00053 CI=[-0.00488,-0.00262]  # 1-seed on this parent; a new incumbent identity may retry
- 152_architecture parent=143_ensemble {'model_family': 'gbm'} dP=-0.02921 CI=[-0.03689,-0.03031]  # 1-seed on this parent; a new incumbent identity may retry

pred_calibration: 14/101 expected_delta within CI, mean_bias=+0.00832 (over-optimistic)

run_knowledge (this job; harness-written; not a human agenda):
- wlr_play 031_watch_time parent=029_ensemble CI_hi<0; 1-seed on that parent only — not a Pure family ban
- wlr_play 032_ablate_c0_s0 parent=031_watch_time CI_hi<0; 1-seed on that parent only — not a Pure family ban
- wlr_play 033_ablate_c0_s1 parent=031_watch_time CI_hi<0; 1-seed on that parent only — not a Pure family ban
- use_beh_rank 044_features parent=039_ensemble CI_hi<0; 1-seed on that parent only — not a Pure family ban
- use_beh_rank 045_ablate_c0_s0 parent=044_features CI_hi<0; 1-seed on that parent only — not a Pure family ban
- use_time_decay 114_features parent=000_fm_baseline CI_hi<0; 1-seed on that parent only — not a static-feature ban
- use_time_decay 115_ablate_c0_s0 parent=114_features CI_hi<0; 1-seed on that parent only — not a static-feature ban
- use_time_decay 116_ablate_c0_s1 parent=114_features CI_hi<0; 1-seed on that parent only — not a static-feature ban
- use_time_decay 117_ablate_c0_s2 parent=114_features CI_hi<0; 1-seed on that parent only — not a static-feature ban

skill_cards (harness-distilled, claims-with-scope):
- claim={'model_family': 'gbm', 'seed': 0} status=falsified-1seed scope=parent=152_architecture evidence=153_ablate_c0_s0 dP=-0.02921  # not a family ban; a new incumbent identity may retry
- claim=complementary-blend status=measured-1seed scope=run evidence=022_ensemble alpha=0.00000 gamma=0.00000 top1=0.52557
- claim=complementary-blend status=measured-1seed scope=run evidence=030_ensemble alpha=0.00000 gamma=0.00000 top1=0.57909
- claim=complementary-blend status=measured-1seed scope=run evidence=040_ensemble alpha=0.00000 gamma=0.00000 top1=0.86511
- claim=complementary-blend status=measured-1seed scope=run evidence=054_ensemble alpha=0.00000 gamma=0.00000 top1=1.00000
- claim=complementary-blend status=measured-1seed scope=run evidence=066_ensemble alpha=0.00000 gamma=0.00000 top1=0.54491
- claim=complementary-blend status=measured-1seed scope=run evidence=077_ensemble alpha=1.00000 gamma=0.00000 top1=0.87189
- claim=complementary-blend status=measured-1seed scope=run evidence=085_ensemble alpha=1.00000 gamma=0.00000 top1=0.87189
- claim=complementary-blend status=measured-1seed scope=run evidence=093_ensemble alpha=0.00000 gamma=0.00000 top1=0.67568
- claim=complementary-blend status=measured-1seed scope=run evidence=103_ensemble alpha=0.00000 gamma=0.00000 top1=0.67568
- claim=complementary-blend status=measured-1seed scope=run evidence=113_ensemble alpha=0.00000 gamma=0.00000 top1=0.62378
- claim=complementary-blend status=measured-1seed scope=run evidence=144_ensemble alpha=0.00000 gamma=0.00000 top1=0.82719

github_hits (persisted; read_paper github/<slug>/README.md, no per-arm quota):
# GitHub hits (this run)

Map mechanisms to legal keys. Do not clone a repo as a trial.

- avinazz3/kuairand-starter-kit https://github.com/avinazz3/kuairand-starter-kit  ★0
- rbrishi15/kuairand-agent https://github.com/rbrishi15/kuairand-agent Autonomous ML research agent for KuaiRand-Pure — TikTok TechJam ★1
- gaozilin2005/track2-kuairand https://github.com/gaozilin2005/track2-kuairand  ★0
- OwenWen00/bytedance-techjam-2026-kuairand https://github.com/OwenWen00/bytedance-techjam-2026-kuairand Recommendation system solution for ByteDance TechJam 2026 using the KuaiRand-Pure dataset. ★0
- Zheyu-Chen-Joey/kuairand-recommendation-search https://github.com/Zheyu-Chen-Joey/kuairand-recommendation-search End-to-end KuaiRand recommendation system with multi-channel recall, LambdaRank, UCB exploration, cold start, bilingual search, and online feedback. ★1

error_memory=(none)

cheap_acts: research=enabled 0/5
diagnose=enabled 0/4 used=(none) legal=user_mixed,sparse_counts
cross_run_graves=5  # CI_hi<0 fingerprints omitted from legal_untried / ablate extras
arms_exhausted=(none)
read_paper_arms_used=(none)
read_paper_files_used=gbm-native/skill.md, readme.md, time-decay/skill.md
legal_skills (index only; load a body with read_paper path=skills/<name>/SKILL.md):
- claims-scope arm=any status=wired keys=(none) | Treat every measurement as claim plus parent scope. Use when a 1-seed CI is negative or a flag looks banned. Do not promote a parent-scoped fail into a family ban.
- gbm-native arm=architecture status=wired keys=model_family, gbm_leaves | LightGBM on un-bucketed numeric columns with small trees. Use when model_family=gbm is already on and gbm_leaves is still default 31. Do not treat a default ID-only GBM as a family ban.
- score-blend arm=ensemble status=wired keys=(none) | Combine diverse ranking scores on valid only. Use when two identities have ≥2 seeds and are not head clones. Do not use ARIMA or time-series forecasts of blend weights.
- steering-rules arm=any status=wired keys=(none) | Short ranking-search steering. Use on plateau or when tempted to add a deep architecture. Do not ingest RecBole or a 200-item generic ML dump.
- time-decay arm=features status=wired keys=use_time_decay, bpr_decay_sample | Causal recency-decay and session momentum versus static ID fields. Use when the features arm still has use_time_decay untried. Do not retry organizer static-ID ablation as this flag.
Do not dump RecBole/Qlib/tsfresh into context. Blend weights are a valid-only grid, not ARIMA.
do_not_emit: read_paper of used files — emit action=improve with config_patch
tried_canonical_patches (banned only on that parent_id; a new incumbent identity may retry the same patch):
- parent=(root) draft: [{'loss': 'bpr_global'}, {'model_family': 'gbm'}]
- parent=007_draft ablate: [{'loss': 'bpr_global'}]
- parent=008_draft ablate: [{'model_family': 'gbm'}, {'loss': 'bpr_global'}]
- parent=020_ensemble features: [{'use_time_decay': True}]
- parent=020_ensemble multitask: [{'aux_click': True}]
- parent=024_features ablate: [{'use_time_decay': True}]
- parent=029_ensemble watch_time: [{'wlr_play': True}]
- parent=031_watch_time ablate: [{'wlr_play': True}, {'loss': 'bpr_global'}]
- parent=039_ensemble features: [{'use_itemcf': True}, {'use_beh_rank': True}]
- parent=044_features ablate: [{'use_beh_rank': True}, {'bpr_decay_sample': True}]
- parent=052_ensemble architecture: [{'arch': 'deepfm'}]
- parent=052_ensemble features: [{'bpr_decay_sample': True}]
- parent=055_crossover ablate: [{'bpr_decay_sample': True}]
- parent=060_architecture ablate: [{'arch': 'deepfm'}]
- parent=065_ensemble capacity: [{'k': 8}]
- parent=065_ensemble features: [{'use_itemcf': True}]
- parent=065_ensemble multitask: [{'aux_click': True}]
- parent=065_ensemble sequence: [{'seq_len': 100, 'seq_mode': 'din'}]
- parent=067_sequence ablate: [{'seq_len': 100, 'seq_mode': 'din'}, {'bpr_pairs_cap': 64}]
- parent=079_features ablate: [{'use_itemcf': True}]
- parent=087_capacity ablate: [{'k': 8}]
- parent=092_ensemble architecture: [{'arch': 'dcnv2'}]
- parent=092_ensemble time_shift: [{'use_hour': True}]
- parent=095_time_shift ablate: [{'use_hour': True}]
- parent=104_architecture ablate: [{'arch': 'dcnv2'}, {'bpr_pairs_cap': 64}]
- parent=000_fm_baseline features: [{'use_time_decay': True}]
- parent=114_features ablate: [{'use_time_decay': True}, {'loss': 'bpr_global'}]
- parent=112_ensemble architecture: [{'model_family': 'torch'}]
- parent=112_ensemble multitask: [{'aux_click': True}]
- parent=112_ensemble time_shift: [{'use_hour': True}]
- parent=122_architecture ablate: [{'model_family': 'torch'}]
- parent=130_time_shift ablate: [{'use_hour': True}, {'bpr_decay_sample': True}]
- parent=138_multitask ablate: [{'aux_click': True}]
- parent=143_ensemble architecture: [{'model_family': 'gbm'}]
- parent=143_ensemble capacity: [{'k': 32}, {'k': 64}]
- parent=143_ensemble loss: [{'bpr_pairs_cap': 64}, {'bpr_pairs_cap': 16}]
- parent=152_architecture ablate: [{'model_family': 'gbm'}]
