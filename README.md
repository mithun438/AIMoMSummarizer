# 🧠 AI MoM - AI-Powered Meeting Summarizer

**AI MoM (AI Minutes of Meeting)** is a Python-based intelligent assistant that automatically generates structured meeting summaries from raw audio/video recordings or transcript files using advanced AI models.

## 📌 Features

- 🎥 Supports video formats: `.mp4`, `.mkv`, `.mov`
- 📄 Accepts text-based formats: `.txt`, `.docx`, `.csv`
- 🧠 Converts meeting recordings into structured summaries using:
  - 🗣️ [OpenAI Whisper](https://github.com/openai/whisper) for transcription
  - 🤖 [Google Gemini 1.5 Pro](https://deepmind.google/technologies/gemini/) for summarization
- ✅ Extracts:
  - Key Discussion Points
  - Decisions Made
  - Action Items (with assignees and deadlines)
  - Technical Terms & Frameworks
  - Risks/Challenges
  - Next Steps
- 📝 Saves the output as a text file

## 🚀 How It Works

1. 📂 Upload a file (video or transcript)
2. 🔍 File type is detected
3. 🎙️ For video: Audio is extracted using `ffmpeg` and transcribed via Whisper
4. 📖 For text: Transcript is read directly
5. 🤖 Google Gemini is used to summarize the transcript intelligently
6. 📄 Summary is printed and saved

## 🛠️ Installation

### On Google Colab:

Run the notebook directly [here](https://colab.research.google.com/drive/1cwA70hLXu1h06b1666ioJ8qJGAUfqjH-).

### Or manually:

```bash
pip install openai-whisper google-generativeai ffmpeg librosa soundfile python-docx pandas
sudo apt-get install ffmpeg
