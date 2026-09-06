<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=rect&color=0:0A2647,100:205295&height=180&section=header&text=Saransh&fontSize=42&fontColor=FFFFFF&fontAlignY=40&desc=NLP-Based%20Text%20Summarization%2C%20Translation%2C%20and%20Text-to-Speech&descSize=16&descAlignY=65" width="100%"/>
</p>

<p align="center">
🔗 <a href="https://github.com/Devanshu1013/Saransh">Original Repository</a> &nbsp;|&nbsp; <a href="https://devanshu1013.github.io/Devanshu_Portfolio/">← Back to Portfolio</a>
</p>

---

## Overview

Saransh (Hindi for "summary") is a text summarization and translation tool that accepts both plain text and PDF input. It uses NLTK-based extractive summarization with lemmatization for improved accuracy, and can output the summary as an audio file — including in multiple languages.

**Highlights:**
- Extracts text directly from PDF documents
- NLTK + lemmatization based extractive summarization with adjustable summary length
- Converts summaries to speech (text-to-audio) using `pyttsx3`
- Translates summaries into multiple languages, with chunked translation for long text

## Background

Long documents — research papers, reports, articles — are often more than most readers want to sit through, but existing summarization tools tend to be single-purpose: they either summarize, or they translate, or they read text aloud, rarely all three together. They also often assume the input is already clean plain text, which breaks down as soon as the source is a PDF with headers, footers, and inconsistent formatting.

Saransh was built to close that gap in one tool: take a document in whatever form it naturally exists (plain text or PDF), condense it to the length the reader actually wants, and then make that summary consumable in more than one way — as text, translated into another language, or as an audio file that can be listened to instead of read. The goal was accessibility as much as convenience: a summary that can be heard, in a language the listener is comfortable with, opens the content up to people who might not otherwise engage with a dense document at all.

## Methodology

**1. Text extraction**
For plain text input, the raw text is used directly. For PDF input, text is extracted using `PyMuPDF`, which pulls the underlying text content directly from the PDF's structure rather than relying on OCR — making it fast and accurate for text-based PDFs (as opposed to scanned image PDFs).

**2. Preprocessing & lemmatization**
Before scoring, the extracted text is cleaned and each word is reduced to its base form via **lemmatization** using NLTK — for example, "running", "ran", and "runs" all reduce to "run". This matters for extractive summarization because it lets the algorithm recognize that different inflections of the same word carry the same topical weight, rather than treating them as unrelated tokens and diluting a sentence's importance score.

**3. Extractive summarization**
Rather than generating new sentences (which risks introducing inaccuracies), Saransh uses an **extractive** approach: it scores each sentence in the source text based on word frequency and importance (using the lemmatized tokens), then selects the highest-scoring sentences to form the summary. The user can adjust the desired summary length, trading off brevity against completeness.

**4. Translation**
Once a summary is generated, it can optionally be translated into another language. Because translation APIs typically have input length limits, long summaries are **chunked** into smaller pieces, translated individually, and then reassembled — preserving translation quality without truncating longer summaries.

**5. Text-to-speech**
The final summary (in the original language or translated) can be converted into an audio file using `pyttsx3`, an offline text-to-speech engine — meaning audio generation doesn't depend on an internet connection or an external API, and works consistently across the languages the summary has been translated into.

## Tech Stack

`Python` `NLTK` `PyMuPDF` `pyttsx3` `Translation`

---

<p align="center">
<a href="https://github.com/Devanshu1013/Devanshu_Portfolio/blob/main/README.md">← Back to Portfolio</a> &nbsp;|&nbsp; 🔗 <a href="https://github.com/Devanshu1013/Saransh">View on GitHub</a>
</p>
