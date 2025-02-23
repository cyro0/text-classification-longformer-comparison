---
library_name: peft
license: apache-2.0
base_model: allenai/longformer-base-4096
tags:
- generated_from_trainer
metrics:
- f1
- accuracy
model-index:
- name: longformer-base-4096-gnad10
  results: []
---

<!-- This model card has been generated automatically according to the information the Trainer had access to. You
should probably proofread and complete it, then remove this comment. -->

# longformer-base-4096-gnad10

This model is a fine-tuned version of [allenai/longformer-base-4096](https://huggingface.co/allenai/longformer-base-4096) on an unknown dataset.
It achieves the following results on the evaluation set:
- Loss: 0.8507
- F1: 0.7045
- Accuracy: 0.7062

## Model description

More information needed

## Intended uses & limitations

More information needed

## Training and evaluation data

More information needed

## Training procedure

### Training hyperparameters

The following hyperparameters were used during training:
- learning_rate: 0.001
- train_batch_size: 8
- eval_batch_size: 8
- seed: 42
- optimizer: Use OptimizerNames.ADAMW_TORCH with betas=(0.9,0.999) and epsilon=1e-08 and optimizer_args=No additional optimizer arguments
- lr_scheduler_type: linear
- num_epochs: 5
- mixed_precision_training: Native AMP

### Training results

| Training Loss | Epoch | Step | Validation Loss | F1     | Accuracy |
|:-------------:|:-----:|:----:|:---------------:|:------:|:--------:|
| 1.3506        | 1.0   | 1156 | 1.2553          | 0.5525 | 0.5652   |
| 1.2343        | 2.0   | 2312 | 0.9642          | 0.6715 | 0.6722   |
| 1.1224        | 3.0   | 3468 | 1.0319          | 0.6367 | 0.6420   |
| 1.0623        | 4.0   | 4624 | 0.8621          | 0.6998 | 0.7043   |
| 1.0311        | 5.0   | 5780 | 0.8507          | 0.7045 | 0.7062   |


### Framework versions

- PEFT 0.14.0
- Transformers 4.48.3
- Pytorch 2.6.0+cu118
- Datasets 3.2.0
- Tokenizers 0.21.0