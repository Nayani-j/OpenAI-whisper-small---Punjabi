# OpenAI-whisper-small---Punjabi
ASR Whisper Model finetuned for Punjabi 
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


Model Link on Hugging Face :https://huggingface.co/nayaniiii/whisper-small-punjabi
