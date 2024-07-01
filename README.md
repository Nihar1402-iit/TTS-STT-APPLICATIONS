# TTS-STT-Voice_cloning

Implemented voice synthesis from text, utilizing deep learning techniques for efficient audio generation. Successfully loaded and utilized pretrained checkpoints for model evaluation and synthesized high-quality speech outputs saved as WAV files.

# Text-to-Speech Generation with Transformers

This repository demonstrates how to generate audio from text using the `transformers` library with the `AutoProcessor` and `BarkModel` from the `suno/bark` model.

## Description

The provided script uses the `suno/bark` model to convert text into speech. The script performs the following steps:
1. Initializes the processor and model from the `suno/bark` pretrained checkpoint.
2. Moves the model to GPU for faster processing.
3. Defines a function `generate_audio` that takes in text, a voice preset, and an output file name.
4. Processes the text and voice preset to prepare inputs for the model.
5. Generates the audio array using the model.
6. Converts the audio array to a numpy array and writes it to a WAV file using the `scipy` library.

## Requirements

- transformers
- scipy
- torch (with CUDA support)
