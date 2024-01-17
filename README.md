# Overview

This Python script implements a simple Speech-to-Text Automatic Speech Recognition (ASR) system using the Google Cloud Speech-to-Text API. It consists of two main functions: convert_to_wav and transcribe_audio.

# convert_to_wav Function

The convert_to_wav function takes an audio file as input and converts it to WAV format with specific parameters using the pydub library. It sets the sample rate to 16,000 Hz, the number of channels to 1 (mono), and the sample width to 2 bytes. The resulting WAV file is saved, and its path is returned.

# transcribe_audio Function

The transcribe_audio function utilizes the convert_to_wav function to convert the input audio file to WAV format. It then uses the Google Cloud Speech-to-Text API to transcribe the speech in the audio file. The function prints the best transcription, alternative transcriptions, and their confidence scores if available. If the API encounters issues during transcription, appropriate error messages are displayed.

# Dependencies

pydub

speech_recognition

# Install the dependencies using:

pip install pydub speech_recognition

# Usage

To use the provided functions:

from your_script_name import convert_to_wav, transcribe_audio

# Convert audio file to WAV
wav_path = convert_to_wav("your_audio_file.mp3")

# Transcribe audio using Google Cloud Speech-to-Text API
transcribe_audio("your_audio_file.mp3")

Notes

Ensure that the necessary libraries are installed using the provided pip install command.

Replace "your_audio_file.mp3" with the path to your actual audio file.
