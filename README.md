# Whisper + GPT

This repository contains three Python application notebooks. The first two are standalone scripts, while the third combines the functionality of the first two into a single script.

The whisper model is used for audio transcription, and the GPT-3.5-turbo model is used for text editing.

These scripts have been tested on Windows 11 with an RTX 3090 and RTX 4090.

See this link for more information on installing whisper local: <https://github.com/openai/whisper/discussions/47>

## Standalone Applications

### 1. Audio Transcription with Whisper

This application transcribes audio files using the Whisper ASR model. The transcriptions are saved to a text file.

#### Usage

- Set the whisper model, "large" is the best performing model.
- Set the `audio_file_path` variable to the path of the audio file you want to transcribe.
- Set the `output_file_path` variable to the path of the text file where you want to save the transcription.
- Run the script, and the transcription will be appended to the output file.

### 2. Revised transcript with GPT-3.5-turbo

This application takes a text file as input, processes it with GPT-3.5-turbo for spelling and grammar corrections, and general text flow and readability, and saves the edited text to a new file.

#### Usage

- Set the `input_text_path` variable to the path of the text file you want to process.
- Set the `output_text_path` variable to the path of the text file where you want to save the edited text.
- Run the script, and the edited text will be saved to the output file.

## Combined Application

The combined application transcribes audio files using the Whisper ASR model, processes the transcriptions with GPT-3.5-turbo for spelling and grammar corrections, and saves both the original and edited transcriptions to separate text files.

#### Usage

- Set the whisper model, "large" is the best performing model.
- Set the `audio_file_path` variable to the path of the audio file you want to transcribe.
- Set the `original_output_file_path` variable to the path of the text file where you want to save the original transcription.
- Set the `revised_output_file_path` variable to the path of the text file where you want to save the revised transcription.
- Run the script, and the original and revised transcriptions will be saved to their respective output files.

## License

This repository is licensed under the MIT license.
