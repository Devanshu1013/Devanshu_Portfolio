<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=rect&color=0:0A2647,100:205295&height=180&section=header&text=Audio%20to%20Text%20Converter&fontSize=30&fontColor=FFFFFF&fontAlignY=40&desc=Lightweight%20Speech-to-Text%20Transcription%20Utility&descSize=16&descAlignY=65" width="100%"/>
</p>

<p align="center">
🔗 <a href="https://github.com/Devanshu1013/Audio_To_Text">Original Repository</a> &nbsp;|&nbsp; <a href="https://devanshu1013.github.io/Devanshu_Portfolio/">← Back to Portfolio</a>
</p>

---

## Overview

A simple utility that converts audio files into text transcripts using the `speech_recognition` library.

**Highlights:**
- Converts spoken audio into text transcripts
- Lightweight, notebook-based implementation

## Background

Not every piece of spoken content comes with a transcript attached — voice memos, recorded lectures, interview recordings, and meeting audio are all common formats that are far easier to search, quote, or archive as text than as raw audio. Manually transcribing even a few minutes of speech is tedious, and most heavyweight transcription tools require cloud APIs, paid services, or complex setup.

This project was built as a lightweight, no-frills answer to that problem: a small utility that takes an audio file and returns its transcript, without requiring anything more than a Python environment and the `speech_recognition` library. The focus was on simplicity and immediate usability over building a production-scale transcription pipeline.

## Methodology

1. **Audio input** — the utility accepts an audio file as input
2. **Preprocessing** — the audio is loaded and prepared in a format compatible with the recognition engine (handling sample rate and channel requirements as needed)
3. **Speech recognition** — the `speech_recognition` library processes the audio, sending it to a recognition backend that converts the spoken audio signal into text
4. **Transcript output** — the resulting transcript is returned as plain text, ready to be copied, saved, or used downstream in another NLP pipeline

The implementation is intentionally kept in a single Jupyter Notebook rather than a full application — favoring quick experimentation and transparency over a polished interface, since the core value here is the transcription logic itself.

## Tech Stack

`Python` `SpeechRecognition` `Jupyter Notebook`

---

<p align="center">
<a href="https://github.com/Devanshu1013/Devanshu_Portfolio/blob/main/README.md">← Back to Portfolio</a> &nbsp;|&nbsp; 🔗 <a href="https://github.com/Devanshu1013/Audio_To_Text">View on GitHub</a>
</p>
