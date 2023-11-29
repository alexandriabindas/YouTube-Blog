---
license: apache-2.0
base_model: distilbert-base-uncased
tags:
- generated_from_trainer
metrics:
- accuracy
model-index:
- name: distilbert-base-uncased-lora-text-classification
  results: []
---

<!-- This model card has been generated automatically according to the information the Trainer had access to. You
should probably proofread and complete it, then remove this comment. -->

# distilbert-base-uncased-lora-text-classification

This model is a fine-tuned version of [distilbert-base-uncased](https://huggingface.co/distilbert-base-uncased) on an unknown dataset.
It achieves the following results on the evaluation set:
- Loss: 0.8839
- Accuracy: {'accuracy': 0.901}

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
- train_batch_size: 4
- eval_batch_size: 4
- seed: 42
- optimizer: Adam with betas=(0.9,0.999) and epsilon=1e-08
- lr_scheduler_type: linear
- num_epochs: 10

### Training results

| Training Loss | Epoch | Step | Validation Loss | Accuracy            |
|:-------------:|:-----:|:----:|:---------------:|:-------------------:|
| No log        | 1.0   | 250  | 0.3334          | {'accuracy': 0.892} |
| 0.3999        | 2.0   | 500  | 0.3850          | {'accuracy': 0.892} |
| 0.3999        | 3.0   | 750  | 0.4382          | {'accuracy': 0.895} |
| 0.2004        | 4.0   | 1000 | 0.5518          | {'accuracy': 0.895} |
| 0.2004        | 5.0   | 1250 | 0.6261          | {'accuracy': 0.899} |
| 0.0674        | 6.0   | 1500 | 0.8357          | {'accuracy': 0.892} |
| 0.0674        | 7.0   | 1750 | 0.8303          | {'accuracy': 0.901} |
| 0.0301        | 8.0   | 2000 | 0.8756          | {'accuracy': 0.894} |
| 0.0301        | 9.0   | 2250 | 0.8779          | {'accuracy': 0.897} |
| 0.0028        | 10.0  | 2500 | 0.8839          | {'accuracy': 0.901} |


### Framework versions

- Transformers 4.35.2
- Pytorch 2.0.1
- Datasets 2.14.4
- Tokenizers 0.15.0
