# OpenAI-whisper-small---Punjabi
ASR Whisper Model finetuned for Punjabi 
---
language:
- pa
license: apache-2.0
tags:
- generated_from_trainer
base_model: openai/whisper-small
datasets:
- mozilla-foundation/common_voice_11_0
metrics:
- wer
model-index:
- name: Whisper Small Punjabi - Nayani Jindal
  results:
  - task:
      type: automatic-speech-recognition
      name: Automatic Speech Recognition
    dataset:
      name: Common Voice 11.0
      type: mozilla-foundation/common_voice_11_0
      config: pa-IN
      split: None
      args: 'config: mr, split: test'
    metrics:
    - type: wer
      value: 49.85875706214689
      name: Wer
---

<!-- This model card has been generated automatically according to the information the Trainer had access to. You
should probably proofread and complete it, then remove this comment. -->

# Whisper Small Punjabi - Nayani Jindal

This model is a fine-tuned version of [openai/whisper-small](https://huggingface.co/openai/whisper-small) on the Common Voice 11.0 dataset.
It achieves the following results on the evaluation set:
- Loss: 0.4789
- Wer: 49.8588

## Model description

More information needed

## Intended uses & limitations

More information needed

## Training and evaluation data

More information needed

## Training procedure

### Training hyperparameters

The following hyperparameters were used during training:
- learning_rate: 1e-05
- train_batch_size: 16
- eval_batch_size: 8
- seed: 42
- optimizer: Adam with betas=(0.9,0.999) and epsilon=1e-08
- lr_scheduler_type: linear
- lr_scheduler_warmup_steps: 500
- training_steps: 1000
- mixed_precision_training: Native AMP

### Training results

| Training Loss | Epoch   | Step | Validation Loss | Wer     |
|:-------------:|:-------:|:----:|:---------------:|:-------:|
| 0.0003        | 16.3934 | 1000 | 0.4789          | 49.8588 |


### Framework versions

- Transformers 4.41.1
- Pytorch 2.1.2
- Datasets 2.19.1
- Tokenizers 0.19.1


Model Link on Hugging Face :https://huggingface.co/nayaniiii/whisper-small-punjabi
