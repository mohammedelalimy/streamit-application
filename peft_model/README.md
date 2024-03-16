---
license: apache-2.0
library_name: peft
tags:
- generated_from_trainer
metrics:
- bleu
base_model: Helsinki-NLP/opus-mt-en-ar
model-index:
- name: finetuned_helsinki_peft_model__en_to_ar
  results: []
---

<!-- This model card has been generated automatically according to the information the Trainer had access to. You
should probably proofread and complete it, then remove this comment. -->

# finetuned_helsinki_peft_model__en_to_ar

This model is a fine-tuned version of [Helsinki-NLP/opus-mt-en-ar](https://huggingface.co/Helsinki-NLP/opus-mt-en-ar) on an unknown dataset.
It achieves the following results on the evaluation set:
- Loss: 1.7655
- Bleu: 26.7751
- Gen Len: 13.524

## Model description

More information needed

## Intended uses & limitations

More information needed

## Training and evaluation data

More information needed

## Training procedure

### Training hyperparameters

The following hyperparameters were used during training:
- learning_rate: 2e-05
- train_batch_size: 24
- eval_batch_size: 24
- seed: 42
- optimizer: Adam with betas=(0.9,0.999) and epsilon=1e-08
- lr_scheduler_type: linear
- lr_scheduler_warmup_steps: 500
- training_steps: 10000
- mixed_precision_training: Native AMP

### Training results

| Training Loss | Epoch | Step  | Validation Loss | Bleu    | Gen Len |
|:-------------:|:-----:|:-----:|:---------------:|:-------:|:-------:|
| 1.9431        | 0.2   | 500   | 1.7705          | 26.9288 | 13.456  |
| 1.9149        | 0.4   | 1000  | 1.7700          | 27.5825 | 13.516  |
| 1.9356        | 0.6   | 1500  | 1.7689          | 26.9314 | 13.5445 |
| 1.9242        | 0.8   | 2000  | 1.7681          | 26.9265 | 13.4585 |
| 1.9542        | 1.0   | 2500  | 1.7686          | 26.9745 | 13.5045 |
| 1.9417        | 1.2   | 3000  | 1.7676          | 27.1966 | 13.545  |
| 1.9233        | 1.4   | 3500  | 1.7675          | 26.7973 | 13.5225 |
| 1.929         | 1.6   | 4000  | 1.7670          | 26.8808 | 13.5455 |
| 1.9504        | 1.8   | 4500  | 1.7669          | 27.0192 | 13.484  |
| 1.9148        | 2.0   | 5000  | 1.7673          | 27.0003 | 13.5225 |
| 1.9052        | 2.2   | 5500  | 1.7667          | 26.9055 | 13.5455 |
| 1.9443        | 2.4   | 6000  | 1.7665          | 26.8744 | 13.492  |
| 1.9212        | 2.6   | 6500  | 1.7667          | 26.7736 | 13.51   |
| 1.9306        | 2.8   | 7000  | 1.7665          | 26.8395 | 13.491  |
| 1.9552        | 3.0   | 7500  | 1.7659          | 26.853  | 13.4695 |
| 1.9396        | 3.2   | 8000  | 1.7653          | 26.7499 | 13.4975 |
| 1.9306        | 3.4   | 8500  | 1.7654          | 26.7146 | 13.53   |
| 1.917         | 3.6   | 9000  | 1.7656          | 26.8062 | 13.527  |
| 1.9285        | 3.8   | 9500  | 1.7655          | 26.7167 | 13.5315 |
| 1.9109        | 4.0   | 10000 | 1.7655          | 26.7751 | 13.524  |


### Framework versions

- PEFT 0.9.1.dev0
- Transformers 4.38.2
- Pytorch 2.1.0+cu121
- Datasets 2.18.0
- Tokenizers 0.15.2