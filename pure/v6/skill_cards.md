# Distilled skill cards (this run)

Harness-written claims-with-scope. Not a to-do list.

skill_cards (harness-distilled, claims-with-scope):
- claim={'loss': 'bpr_global', 'seed': 0} status=confirmed-3seed scope=parent=007_draft evidence=009_ablate_c0_s0 mean=0.60282
- claim={'arch': 'deepfm', 'seed': 0} status=confirmed-3seed scope=parent=018_architecture evidence=019_ablate_c0_s0 mean=0.60339
- claim={'seq_len': 100, 'seq_mode': 'pool', 'seed': 0} status=confirmed-3seed scope=parent=044_sequence evidence=045_ablate_c0_s0 mean=0.60396
- claim={'seq_len': 20, 'seq_mode': 'din'} status=falsified-1seed scope=parent=045_ablate_c0_s0 evidence=103_sequence dP=-0.00138  # not a family ban; a new incumbent identity may retry
- claim={'seq_len': 10, 'seq_mode': 'pool'} status=falsified-1seed scope=parent=045_ablate_c0_s0 evidence=133_sequence dP=-0.00204  # not a family ban; a new incumbent identity may retry
- claim=complementary-blend status=measured-1seed scope=run evidence=015_ensemble alpha=0.00000 gamma=0.00000 top1=0.81018
- claim=complementary-blend status=measured-1seed scope=run evidence=027_ensemble alpha=0.00000 gamma=0.00000 top1=0.80715
- claim=complementary-blend status=measured-1seed scope=run evidence=037_ensemble alpha=0.00000 gamma=0.00000 top1=0.86040
- claim=complementary-blend status=measured-1seed scope=run evidence=053_ensemble alpha=0.00000 gamma=0.00000 top1=0.85650
- claim=complementary-blend status=measured-1seed scope=run evidence=064_ensemble alpha=0.00000 gamma=0.00000 top1=0.85991
- claim=complementary-blend status=measured-1seed scope=run evidence=093_ensemble alpha=0.00000 gamma=0.00000 top1=0.82709
- claim=complementary-blend status=measured-1seed scope=run evidence=114_ensemble alpha=0.00000 gamma=0.00000 top1=0.81631
