# Skips, duplicates, errors

- `007_draft` arm=draft skip=False error=nonzero_exit
- `008_debug` arm=draft skip=True error=debug noop; refusing to retrain the parent config
- `025_crossover` arm=features skip=False error=data_scale=pure not on disk
- `026_sequence` arm=sequence skip=False error=data_scale=pure not on disk
- `027_architecture` arm=architecture skip=False error=data_scale=pure not on disk
- `029_regularization` arm=regularization skip=False error=data_scale=pure not on disk
- `030_loss` arm=loss skip=False error=data_scale=pure not on disk
- `031_sequence` arm=sequence skip=False error=data_scale=pure not on disk
- `033_regularization` arm=regularization skip=True error=duplicate of 029_regularization
- `035_architecture` arm=architecture skip=False error=timeout
- `036_architecture` arm=architecture skip=False error=timeout
- `037_sequence` arm=sequence skip=False error=data_scale=pure not on disk
- `048_loss` arm=loss skip=False error=data_scale=pure not on disk
- `049_architecture` arm=architecture skip=False error=timeout
- `050_regularization` arm=regularization skip=False error=data_scale=pure not on disk
- `051_architecture` arm=architecture skip=False error=data_scale=pure not on disk
- `053_architecture` arm=architecture skip=False error=timeout
