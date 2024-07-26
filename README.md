# TTS-STT_APLICATIONS

## Video to Audio Text Analysis and Synthesis

This project provides a comprehensive solution to process video files by converting them into audio, transcribing the audio to text, summarizing the text, performing sentiment analysis, and generating text-to-speech outputs. It uses a combination of libraries including MoviePy, SpeechRecognition, Hugging Face Transformers, and gTTS.

### Features

- **Video to Audio Conversion:** Extracts audio from MP4 video files and saves it as WAV format.
- **Speech-to-Text:** Converts the extracted audio into text using Google’s Speech Recognition API.
- **Text Summarization:** Summarizes the transcribed text to provide concise information.
- **Sentiment Analysis:** Analyzes the sentiment of the summarized text to classify the working environment.
- **Text-to-Speech:** Converts the summarized text into an audio file using Google Text-to-Speech (gTTS).

Implemented voice synthesis from text, utilizing deep learning techniques for efficient audio generation. Successfully loaded and utilized pretrained checkpoints for model evaluation and synthesized high-quality speech outputs saved as WAV files.

## Code Explanation

- **`mp4_to_wav(mp4_file, wav_file)`:** Converts MP4 video to WAV audio.
- **`speech_to_text(wav_file)`:** Transcribes the WAV audio to text using SpeechRecognition.
- **`summarize_text(text)`:** Summarizes the transcribed text using Hugging Face Transformers.
- **`analyze_sentiment(text)`:** Analyzes the sentiment of the summarized text using a pre-trained model.
- **`classify_working_environment(sentiment_label, sentiment_score)`:** Classifies the working environment based on sentiment analysis results.
- **`text_to_speech(text, tts_file)`:** Converts the summarized text into speech and saves it as an MP3 file.
  
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
